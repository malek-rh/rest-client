#XMLFormat used by RESTClient.

# Request XML #

```
<?xml version="1.0" encoding="UTF-8" standalone="no"?>
<rest-client version="2.0">
 <request>
  <URL>http://wiztools.org/</URL>
  <method>GET</method>
  <auth-methods>BASIC,DIGEST</auth-methods>
  <auth-preemptive>false</auth-preemptive>
  <auth-host>wiztools.org</auth-host>
  <auth-realm>/sma/api/rest</auth-realm>
  <auth-username>subwiz</auth-username>
  <auth-password>rO0ABXQACHBhc3N3b3Jk</auth-password>
  <headers>
   <header key="key" value="value"/>
  </headers>
  <body charset="UTF-8" content-type="text/plain">Request body content</body>
 </request>
</rest-client>
```


# Response XML #

```
<?xml version="1.0" encoding="UTF-8" standalone="no"?>
<rest-client version="2.0">
 <response>
  <status code="200">Ok</status>
  <headers>
   <header key="key" value="value"/>
  </headers>
  <body>Response body content</body>
 </response>
</rest-client>
```