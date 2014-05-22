PragmaMS
========

The Pragma Media Server - the pragmatic media server. If you can talk the talk. You can walk the walk.

## Basic philosophy
The Pragma Media Server should make your media searchable and cachable (where relevant). It will be implemented as a sett of [Docker](http://docker.io) containers and distributed as Docker-files. PragmaMS will standardize a set of media operations as a set of GETs over http/https. The standard is the "talk". Underlying systems will do the actual operations on the media ("the walk"). It will come with "batterys included". Underlying system should be easy to replace as long as the GETs can be translated and passed on.

## An outline so fare
* [Pound] to handle https
* [Varnish cache] with persistant file storage to handle caching of dynamicly constructed content (resized images ...) and rewrite of GETs to underlaying systems.
* [EXIFTools] to get metadata from uploaded media files
* [Elasticsearch] for metadata search
* [Nginx] (with relevant modules) as basic webserver and media server
* [Web2py] for webinterface
* [IIPImage] for zoomable images
* [YouTube] for video
* [Vimeo] for video
* [Flickr] for images
* [Slideshare] for presentations
* [Prezi] for prezies
* [Amazone S3] or eqvivalent for storing uploaded media files
