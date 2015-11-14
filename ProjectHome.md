## Overview: ##
FeedReader is a C++ library designed to retrieve and parse [web feeds](http://en.wikipedia.org/wiki/Web_feed) such as [RSS](http://en.wikipedia.org/wiki/RSS_(file_format)), [ATOM](http://en.wikipedia.org/wiki/ATOM) and [RDF](http://en.wikipedia.org/wiki/Resource_Description_Framework).



## Features: ##
FeedReader was designed to scale: it is _fast_, _thread-safe_, _extensible_ and _platform-independent_.

In FeedReader, all feeds are transformed via XSL to a uniform schema before being parsed. This means that in order to extend FeedReader to support a new feed format, all that is needed is a new XSL file.
The library comes with XSL files supporting for the following feed formats:
  * RSS 1.0
  * RSS 2.0
  * ATOM 0.3
  * ATOM 1.0
  * RDF

An iterator interface is provided to the feed elements parsed.

Using the library is simple, sample client code is available [here](sample_client_code.md).

## Dependencies: ##
The FeedReader library is dependent on, and was tested with the following libraries/versions:
  * [Boost](http://www.boost.org/users/news/version_1_36_0) 1.36 (was also tested with 1.33\_1)
  * [libcurl](http://curl.haxx.se/) 7.18.1
  * [Xerces](http://xerces.apache.org/xerces-c/) 2.8.0
  * [Xalan](http://xml.apache.org/xalan-j/) 1.10.1
  * [Zlib](http://www.zlib.net/) 1.23 (required by CURL)



## About: ##
_FeedReader was created by Yoav Aviram (yoav.aviram AT gmail DOT com)._

Patches and bug reports are welcome, just please keep the style consistent with the original source.