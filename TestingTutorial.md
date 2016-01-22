#Tutorial on writing a simple TestCase

# Introduction #

This is a quick tutorial on writing TestCases using REST Client 3.0.

# Details #

REST Client has Groovy embedded. Groovy supports JUnit 3.x type test cases (if you don't know what it means, just chill, because I will be explaining this shortly).

# Writing Test Class #

```
public class MyTest extends org.wiztools.restclient.RESTTestCase{

 /* TEST METHODS */

}
```

# A Sample Test Method #

All test methods should be named with prefix `test`. A sample test method which tests if the response body contains the text `WizTools.org`:

```
public void testRequestContainsWizTools(){
  if(response.getResponseBody() != null
      && (new String(response.getResponseBody(), "UTF-8").indexOf("WizTools.org") > -1)){
    // do nothing!
  }
  else{
    fail("Response body does not have `WizTools.org' text.");
  }
}
```

Two instance variables `request` and `response` with prepopulated data is available for the test script. The methods that can be invoked on these objects are detailed here: http://code.google.com/p/rest-client/wiki/TestClass.

After making the request, the Response Test Result tab will show the result of executing the Test Script. Change the text `WizTools.org` to `ABC2XYZ`. Now place the request again, this would fail the test, and be reported in the Response Test Result tab.

The sample request is available here: http://rest-client.googlecode.com/files/sample-test-request-30.rcq. Download this and save to your local drive. Then open this file using `File>Open Request` in RESTClient interface.