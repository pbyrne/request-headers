Request Headers
===============

Basic server which reports the HTTP request headers it receives.
Useful for testing load balancers or reverse proxies to ensure that you're setting the headers you want.

Usage
-----

```
request-headers
```

Listens on port 5000.

Example
-------

```
$ curl -H "HTTP-X-Foo: example" -H "Foo: bar" -H "Foo: baz" http://0.0.0.0:5000/
Accept: [*/*]
Foo: [bar baz]
Http-X-Foo: [example]
User-Agent: [curl/7.37.1]
```
