To write a simple request and write the response body to standard out.

# Introduction #

Make sure you have configured your CLASSPATH/build environment (maven) as specified in [Extending](Extending.md).


# Details #

## Create Request ##

First create the Request object:

```
import org.wiztools.restclient.bean.Request;
import org.wiztools.restclient.bean.RequestBean;
import org.wiztools.restclient.bean.HTTPMethod;

...

RequestBean requestBean = new RequestBean();
requestBean.setUrl(new java.net.URL("http://wiztools.org/"));
requestBean.setMethod(HTTPMethod.GET);

// Optional: assign implementation to interface:
Request request = requestBean;
```

## Create Handler ##

This handler will print the response body to STDOUT.

```
import org.wiztools.restclient.View;

...

View view = new View(){
  @Override
  public void doStart(Request request){
    // do nothing!
  }

  @Override
  public void doResponse(Response response){
    System.out.println(response.getResponseBody());
  }

  @Override
  public void doCancelled(){
    // do nothing!
  }

  @Override
  public void doEnd(){
    // do nothing!
  }

  @Override
  public void doError(final String error){
    System.err.println(error);
  }
};
```

## Execute the request ##

```
import org.wiztools.restclient.bean.RequestExecuter;
import org.wiztools.restclient.ServiceLocator;

...

RequestExecuter executer = ServiceLocator.getInstance(RequestExecuter.class);

// 'request' and 'view' are the objects created in the previous sections:
executer.execute(request, view);
```

**Note**: The implementation of the RequestExecuter interface stores state data. So do not cache _executer_ object. Each time you need to execute a request, make a call to _ServiceLocator.getInstance(RequestExecuter.class)_.