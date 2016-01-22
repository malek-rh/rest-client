#How to read and write Request and Response to file system.

# Introduction #

One of the main features of RESTClient is its ability to persist Request and Response objects to filesystem. In this recipe we will show you how to do it using RESTClient API.


# Details #

## Writing to a file ##

```
import org.wiztools.restclient.util.XMLUtil;
import org.wiztools.restclient.XMLException;
import org.wiztools.restclient.bean.Request;
import org.wiztools.restclient.bean.Response;
import java.io.IOException;

...

Request request = ...;
Response response = ...;

try{
  XMLUtil.writeRequestXML(request, new File("req.rcq"));
  XMLUtil.writeResponseXML(response, new File("res.rcs"));
} catch(IOException ex){
  // Handle Exception
} catch(XMLException ex){
  // Handle Exception
}
```

## Reading from file ##

```
import org.wiztools.restclient.util.XMLUtil;
import org.wiztools.restclient.XMLException;
import org.wiztools.restclient.bean.Request;
import org.wiztools.restclient.bean.Response;
import java.io.IOException;

...

try{
  Request request = XMLUtil.getRequestFromXMLFile(new File("req.rcq"));
  Response response = XMLUtil.getResponseFromXMLFile(new File("res.rcs"));
} catch(IOException ex){
  // Handle Exception
} catch(XMLException ex){
  // Handle Exception
}
```