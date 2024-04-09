Introduction
=================
## No SSL = No cry

**Forked from  https://github.com/addisonElliott/HttpServer**
Removed ZLIB and SSL libraries for pure Qt support. Due to this limitations this HttpSever edition suits well for development purposes and 
embedding into other systems for internal API use only. For production when end users have access to content please use [original HttpServer](https://github.com/addisonElliott/HttpServer)

HttpServer is a C++ library that uses the Qt platform to setup a feature rich, easy-to-use HTTP server.


Features
=================
* Single-threaded with asynchronous callbacks
* HTTP/1.1
* ~~TLS support~~ For TLS support please use [original HttpServer](https://github.com/addisonElliott/HttpServer)
* ~~Compression & decompression (GZIP-only)~~ For GZIP support please use [original HttpServer](https://github.com/addisonElliott/HttpServer)
* Easy URL router with regex matching
* Form parsing (multi-part and www-form-urlencoded)
* Sending files
* JSON sending or receiving support
* Custom error responses (e.g. HTML page or JSON response)

Promises Support
=================
There are two variants of this library, one with and without promise support. Promises allow for easier & cleaner development with asynchronous logic. The two variants are supported via separate branches:

1. **master** - No promise support
2. **promises** - Promise support

**Note:** The variant without promise support is considered deprecated and will only be supported via bug fixes in the future. For new development, promises are encouraged. The code will remain in two separate branches until sufficient unit testing & documentation is provided for promises support. If you would like to help, please contribute!

Installing
=================
Prerequisites
-------------
* Qt (tested on 5.15.13, should work on a 6.x also)
* QtPromise for promise support (see [here](https://qtpromise.netlify.app/qtpromise/getting-started.html#installation) for installation instructions)

Building HttpServer
-------------------------
1. qmake -project
2. qmake
3. make (nmake)
4. or through Qt Creator

License
=================
HttpServer has an MIT-based [license](https://github.com/addisonElliott/HttpServer/blob/master/LICENSE).
