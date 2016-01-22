#RESTClient Test Class

# Writing RESTClient Test Class #

The Test Class should follow JUnit convention (JUnit 4.x support is still not present). But instead of extending your class from `junit.framework.TestCase`, it needs to be extended from `org.wiztools.restclient.RESTTestCase`.

Two pre-populated read-only objects are available in the instance for validating test results:

  * request
  * response

## request ##

All the public methods defined in this interface may be invoked:

http://code.google.com/p/rest-client/source/browse/restclient-lib/src/main/java/org/wiztools/restclient/bean/Request.java

## response ##

All public methods defined in this interface may be invoked:

http://code.google.com/p/rest-client/source/browse/restclient-lib/src/main/java/org/wiztools/restclient/bean/Response.java