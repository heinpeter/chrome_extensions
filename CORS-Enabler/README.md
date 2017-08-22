<h1><img src="resources/icon.png" height="64" width="64"/> Chrome-Extension-CORS-Enabler</h1>

CORS is acronyms for Cross-Origin-Resources-Sharing 
(Learn More: https://en.wikipedia.org/wiki/Cross-origin_resource_sharing )

This Chrome-extension will remove the following headers (not case-sensitive):
- access-control-allow-origin
- access-control-allow-headers
- access-control-expose-headers
- access-control-allow-credentials
- access-control-allow-methods
- timing-allow-origin
- content-security-policy
- content-security-policy-report-only
- frame-options
- strict-transport-security
- x-content-security-policy
- x-content-type-options
- x-csp
- x-frame-options
- x-webkit-csp
- x-xss-protection
- x-ua-compatible

and will write the following headers (instead):

<pre>
Access-Control-Allow-Origin       *
Access-Control-Allow-Headers      Accept, Accept-Charset, Accept-Encoding, Accept-Language, Access-Control-Allow-Credentials, Access-Control-Allow-Headers, Access-Control-Allow-Methods, Access-Control-Allow-Origin, Access-Control-Expose-Headers, Access-Control-Max-Age, Access-Control-Request-Headers, Access-Control-Request-Method, Cache-Control, Connection, Content-Description, Content-Encoding, Content-Language, Content-Length, Content-Transfer-Encoding, Content-Type, Cookie, Date, DNT, Expires, Host, If-Modified-Since, Keep-Alive, Last-Modified, Origin, Pragma, Referer, Remote-Address, Server, Set-Cookie, Timing-Allow-Origin, Transfer-Encoding, User-Agent, Vary, X-Content-Type-Options, X-CustomHeader, X-Forwarded-For, X-Forwarded-Host, X-Forwarded-Port, X-Forwarded-Proto, X-Forwarded-Server, X-HTTP-Method-Override, X-Modified, X-OTHER, X-PING, X-PINGOTHER, X-Powered-By, X-Real-IP, X-Requested-With
Access-Control-Expose-Headers     Accept, Accept-Charset, Accept-Encoding, Accept-Language, Access-Control-Allow-Credentials, Access-Control-Allow-Headers, Access-Control-Allow-Methods, Access-Control-Allow-Origin, Access-Control-Expose-Headers, Access-Control-Max-Age, Access-Control-Request-Headers, Access-Control-Request-Method, Cache-Control, Connection, Content-Description, Content-Encoding, Content-Language, Content-Length, Content-Transfer-Encoding, Content-Type, Cookie, Date, DNT, Expires, Host, If-Modified-Since, Keep-Alive, Last-Modified, Origin, Pragma, Referer, Remote-Address, Server, Set-Cookie, Timing-Allow-Origin, Transfer-Encoding, User-Agent, Vary, X-Content-Type-Options, X-CustomHeader, X-Forwarded-For, X-Forwarded-Host, X-Forwarded-Port, X-Forwarded-Proto, X-Forwarded-Server, X-HTTP-Method-Override, X-Modified, X-OTHER, X-PING, X-PINGOTHER, X-Powered-By, X-Real-IP, X-Requested-With
Access-Control-Allow-Methods      CONNECT, DEBUG, DELETE, GET, HEAD, OPTION, PATCH, PING, POST, PUT, TRACE, TRACK
Access-Control-Allow-Credentials  true
Timing-Allow-Origin               *
</pre>

- The CORS above is a result of a resource I've done some time ago, and you could read all about it here: http://icompile.eladkarako.com
- You will not see it in the developer-tools/network tab, CORS effects XHR (XML-HTTP-Requests done from the page's body)

it is useful if you plan-on creating a "proxy" but you want to test-thing-up before, with JavaScript.

<h3>This Extension Is A Great Way To Enhance/Ease Client-Side Web-Programming.</h3>

<hr/>


<hr/>

<pre>
Developer's HUB / Changelog

1.0.0.3
* engine update - "try/catch" wrap HTTP-headers modification code-block, to test and see of overriding HTTP-headers, previously overridden from another extension can be silently handled (NOPE! but kept try/catch wrapping :| ).

1.0.0.1
+ initial (no versioning while product was in-alpha developing :/ ).
</pre>

<!-- <a href="https://paypal.me/e1adkarak0"><img src="https://www.paypalobjects.com/webstatic/mktg/Logo/pp-logo-100px.png" alt="PayPal Donation"></a> -->