# Release Notes #

# v 3.3 (Upcoming) #

  * [Issue 198](https://code.google.com/p/rest-client/issues/detail?id=198) NPE when body is not present.
  * [Issue 200](https://code.google.com/p/rest-client/issues/detail?id=200) Optimized HTML syntax color support added.
  * [Issue 193](https://code.google.com/p/rest-client/issues/detail?id=193) Windows test failure.
  * [Issue 203](https://code.google.com/p/rest-client/issues/detail?id=203) NFE in cli when RESTClient cli is run fresh (~/.rest-client/ does not exist).
  * [Issue 206](https://code.google.com/p/rest-client/issues/detail?id=206) SslReqBean trustStore and keyStore type changed to java.io.File.

# v 3.2.2 #

  * [Issue 171](https://code.google.com/p/rest-client/issues/detail?id=171) Response body in HEX format--wrong parsing of Content-type header.
  * [Issue 189](https://code.google.com/p/rest-client/issues/detail?id=189) Updated osxappbundle-maven-plugin to latest fork version.
  * [Issue 190](https://code.google.com/p/rest-client/issues/detail?id=190) XML-Indentation changes encoding to UTF-16.
  * [Issue 191](https://code.google.com/p/rest-client/issues/detail?id=191) Loss of precision in float types during JSON indentation.
  * [Issue 192](https://code.google.com/p/rest-client/issues/detail?id=192) Support for HTML indentation.
  * [Issue 196](https://code.google.com/p/rest-client/issues/detail?id=196) Stretched UI.
  * [Issue 157](https://code.google.com/p/rest-client/issues/detail?id=157) Response body size in status bar.

# v 3.2.1 #

  * [Issue 181](https://code.google.com/p/rest-client/issues/detail?id=181) Groovy Test Scripts Support for external Jars.
  * [Issue 183](https://code.google.com/p/rest-client/issues/detail?id=183) IDN URLs after application restart are corrupted.
  * [Issue 180](https://code.google.com/p/rest-client/issues/detail?id=180) Proxy configuration was not working in cli.

# v 3.2 #

  * [Issue 146](https://code.google.com/p/rest-client/issues/detail?id=146) History support added.
  * [Issue 163](https://code.google.com/p/rest-client/issues/detail?id=163) Cli tool now supports saving response body only.
  * [Issue 173](https://code.google.com/p/rest-client/issues/detail?id=173) Internationalized Domain Name (IDN) support.
  * [Issue 175](https://code.google.com/p/rest-client/issues/detail?id=175) Persist drop-down list of URLs

# v 3.1 #

  * [Issue 100](https://code.google.com/p/rest-client/issues/detail?id=100) Multipart request body support.
  * [Issue 156](https://code.google.com/p/rest-client/issues/detail?id=156) Copy cookie name-value pairs in response header added.
  * [Issue 155](https://code.google.com/p/rest-client/issues/detail?id=155) Requests with auth elements when saved, were not openable.
  * URL request body support.
  * New tool accessible from menu for URL encoding / decoding.

# v 3.0 #

  * [Issue 112](https://code.google.com/p/rest-client/issues/detail?id=112) Unable to correct case in URL fixed.
  * [Issue 19](https://code.google.com/p/rest-client/issues/detail?id=19) [Issue 93](https://code.google.com/p/rest-client/issues/detail?id=93) Binary request body support added
  * [Issue 19](https://code.google.com/p/rest-client/issues/detail?id=19) Added checkbox to ignore response body.
  * [Issue 33](https://code.google.com/p/rest-client/issues/detail?id=33) Added support for PATCH method.
  * [Issue 101](https://code.google.com/p/rest-client/issues/detail?id=101) NTLM support added, but NOT tested (yet).
  * [Issue 145](https://code.google.com/p/rest-client/issues/detail?id=145) OAuth Bearer support.
  * Jetty version updated to latest.
  * [Issue 147](https://code.google.com/p/rest-client/issues/detail?id=147) DELETE method to support body.
  * [Issue 137](https://code.google.com/p/rest-client/issues/detail?id=137) Separate cookie tab.
  * [jsyntaxpane](http://jsyntaxpane.googlecode.com/) dependency removed and replaced with [RSyntaxTextArea](http://fifesoft.com/rsyntaxtextarea/)

# v 2.5 #

  * Dialog box'es Ok button configured to be _default button_---this enables pressing Enter in the dialog to accept it.
  * [Issue 144](https://code.google.com/p/rest-client/issues/detail?id=144) TLS mutual authentication patch from [Matt Wilson](http://mattwilson.org/).
  * Dependencies upgraded to latest version: JSyntaxPane [Issue 86](https://code.google.com/p/rest-client/issues/detail?id=86), Apache HTTPClient, Jackson, and swing auto-complete components.
  * [Issue 138](https://code.google.com/p/rest-client/issues/detail?id=138) Recent file list availability in menu.
  * Google Guice introduced in codebase.
  * [Issue 132](https://code.google.com/p/rest-client/issues/detail?id=132): Updated code to correct implementation of Base64 encoding.
  * [Issue 143](https://code.google.com/p/rest-client/issues/detail?id=143) & [Issue 135](https://code.google.com/p/rest-client/issues/detail?id=135) Support added for self-signed certs.

# v 2.4 #

  * Enhanced Mac support
  * Pressing Enter key in address bar triggers request
  * Ctrl + L or Cmd +L brings focus to the address bar
  * Address bar text is selected completely when focus is gained
  * Redirects can be turned off (option available in Etc. panel in Request)
  * Dependency libraries upgraded to latest versions
  * Other minor bug fixes

# v 2.3.3 #

  * Various charset related issues fixed: [Issue 120](https://code.google.com/p/rest-client/issues/detail?id=120), [Issue 116](https://code.google.com/p/rest-client/issues/detail?id=116), [Issue 114](https://code.google.com/p/rest-client/issues/detail?id=114), [Issue 122](https://code.google.com/p/rest-client/issues/detail?id=122) and [Issue 123](https://code.google.com/p/rest-client/issues/detail?id=123).
  * [Issue 113](https://code.google.com/p/rest-client/issues/detail?id=113) Hostname Verifier option was being ignored in few cases. Fixed.

# v 2.3.2 #

  * Internal code optimization by utilizing the [WizTools.org Commons Lib](http://wiztools-commons-lib.googlecode.com/)
  * Now accepts headers and parameters with multiple values with identical keys.

# v 2.3.1 #

  * Response body encoding is not taken as UTF-8 by default.

# v 2.3 #

  * [Issue 70](https://code.google.com/p/rest-client/issues/detail?id=70) Preemptive authentication was not working. Now fixed.
  * [Issue 64](https://code.google.com/p/rest-client/issues/detail?id=64) Cancel button in Options panel was throwing Exception in certain cases. Fixed.
  * Test results are now shown with more detail than in previous editions.
  * XML parsing changed to Elliotte Rusty Harold's XOM. Much more maintainable. Thanks to @velrajan.r for contributing to this code.
  * [Issue 44](https://code.google.com/p/rest-client/issues/detail?id=44) Now it is possible to cancel a request in the midst of execution. Thanks to Java Concurrency in Practice book.
  * [Issue 71](https://code.google.com/p/rest-client/issues/detail?id=71) Http Response body is searchable -- press Ctrl + F with the focus in that section. (This feature is implemented in JSyntaxPane project. Any bugs, please report there.)
  * [Issue 73](https://code.google.com/p/rest-client/issues/detail?id=73) Font can be specified in Response body component. Previously, because of this limitation, it was not possible to test other language (eg. Chinese) services.
  * [Issue 72](https://code.google.com/p/rest-client/issues/detail?id=72) Automatic indentation of response body support added.
  * OptionsDialog refactored for extensibility.
  * [Issue 75](https://code.google.com/p/rest-client/issues/detail?id=75) Ajax-type auto-complete support added in combo boxes.
  * Better separation of implementation classes and interfaces using the new Object creation class Implementation.of().
  * [Issue 78](https://code.google.com/p/rest-client/issues/detail?id=78) Command-line interface added.
  * [Issue 37](https://code.google.com/p/rest-client/issues/detail?id=37) SSL Hostname verification: different options added.
  * Re-organize the code into different independent modules. Made highly extensible.
  * Added Cookbook section in Wiki.

# v 2.2 #

  * Trace Server port can be configured using system property.
  * Groovy updated to newer version (1.5.6).
  * [Issue 68](https://code.google.com/p/rest-client/issues/detail?id=68) HTTPClient updated to version 4.0-beta1.
  * [Issue 69](https://code.google.com/p/rest-client/issues/detail?id=69) JSON indent support added.

# v 2.2a2 #

This is an Alpha release for public testing.

Changes im this release:
  * Jetty embedded for quick testing.
  * [Issue 65](https://code.google.com/p/rest-client/issues/detail?id=65) The content type and charset of request body was always being set to text/plain and UTF-8 inspite of setting different value in the UI. Fixed.
  * [Issue 66](https://code.google.com/p/rest-client/issues/detail?id=66) Added MIME type 'application/x-www-form-urlencoded' to list of types.

# v 2.2a1 #

This is an Alpha release for public testing.

Changes in this release:
  * HTTP library changed from Commons HTTP to Apache HTTP Client.
  * Syntax highlighting Text editor added.
  * SSL certificate support added.
  * HTTP version can be specified in request.
  * Many UI changes for usability.