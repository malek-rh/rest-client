#How to use WizTools.org RESTClient APIs to program your own interface for it.

# Introduction #

WizTools.org RESTClient initially started as a Swing application to visually test RESTful webservice. With the development catching heat, and increased public interest, the tool required to accommodate various new features. I have also been presented RESTClient modified code by other developers which have been exactly customized for their particular need. So far this has been not too difficult, but it is now made much more easier.

Now, the code is divided into the following modules:

  * _restclient-server_: Jetty embedded code for use in testing and for use in restclient-ui module.
  * _restclient-lib_: This should be the primary module the developers interested in extending RESTClient should focus on.
  * _restclient-ui_: This is the Swing part of RESTClient.
  * _restclient-cli_: This is the command-line tool to execute saved requests.

# Using restclient-lib in your Maven project #

First checkout the source code from svn, then do:

```
$ cd restclient-server
$ mvn install
$ cd ../restclient-lib
$ mvn install
```

This will install the restclient-lib module in your local Maven repository. Now in your project add the dependency:

```
<dependency>
  <groupId>org.wiztools.restclient</groupId>
  <artifactId>restclient-lib</artifactId>
  <version>2.3</version>
</dependency>
```

# The lib API #

The API is not published in a publicly accessible HTTP server right now. But the code itself can be seen here:

http://code.google.com/p/rest-client/source/browse/#git%2Frestclient-lib%2Fsrc%2Fmain%2Fjava%2Forg%2Fwiztools%2Frestclient

# The interfaces and classes you need to know #

To extend RESTClient the following interfaces and classes you need to know:

  * [RequestExecuter](http://code.google.com/p/rest-client/source/browse/restclient-lib/src/main/java/org/wiztools/restclient/bean/RequestExecuter.java): This interface is used to execute the request.
  * [View](http://code.google.com/p/rest-client/source/browse/restclient-lib/src/main/java/org/wiztools/restclient/View.java): This is the callback interface which you have to implement to handle response from the server.
  * [Request](http://code.google.com/p/rest-client/source/browse/restclient-lib/src/main/java/org/wiztools/restclient/bean/Request.java): This is the interface for Request.
  * [RequestBean](http://code.google.com/p/rest-client/source/browse/restclient-lib/src/main/java/org/wiztools/restclient/bean/RequestBean.java): An implementation of Request.
  * [Response](http://code.google.com/p/rest-client/source/browse/restclient-lib/src/main/java/org/wiztools/restclient/bean/Response.java): The Response interface. An implementation of this will be holding the server response.

# Example #

See [ExtendingFirstExample](ExtendingFirstExample.md).