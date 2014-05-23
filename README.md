PragmaMS
========

The Pragma Media Server - the pragmatic media server. If you can talk the talk. You can walk the walk.

## Basic philosophy
The Pragma Media Server should make your media searchable and cachable (where relevant). It will be implemented as a sett of [Docker](http://docker.io) containers and distributed as Docker-files. PragmaMS will standardize a set of media operations as a set of GETs over http/https. The standard is the "talk". Underlying systems will do the actual operations on the media ("the walk"). It will come with "batterys included". Underlying system should be easy to replace as long as the GETs can be translated and passed on.

## An outline so fare
* [Pound](http://www.apsis.ch/pound/) to handle https
* [Varnish cache](https://www.varnish-cache.org/) with persistant file storage to handle caching of dynamicly constructed content (resized images ...) and rewrite of GETs to underlaying systems.
* [EXIFTool](http://owl.phy.queensu.ca/~phil/exiftool/) to get metadata from uploaded media files
* [Elasticsearch](http://www.elasticsearch.org/) for metadata search
* [Nginx](http://nginx.org/) (with relevant modules) as basic webserver and media server
* [Web2py](http://www.web2py.com/) for webinterface
* [IIPImage](http://iipimage.sourceforge.net/) for zoomable images
* [YouTube](https://www.youtube.com/) for video
* [Vimeo](https://vimeo.com/) for video
* [Flickr](https://www.flickr.com/) for images
* [Slideshare](http://www.slideshare.net/) for presentations
* [Prezi](http://prezi.com/) for prezies
* [Amazon S3](http://aws.amazon.com/s3/) or eqvivalent for storing uploaded media files
