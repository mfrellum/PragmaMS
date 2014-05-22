PragmaMS
========

The Pragma Media Server - the pragmatic media server. If you can talk the talk. You can walk the walk.

## Basic philosopy
The Pragma Media Server should make your media searchable and cachable (where relevant). It will be implemented as a sett of Docker containers and distributed as Docker-files. PragmaMS will standardize a set of media operations as a set of GETs over http/https. The standard is the "talk". Underlying systems will do the actual operations on the media. It should be easy to change the underlying system as long as the GETs can be translated so the underlying system can do the work ("the walk").

## An outline so fare
*Pound to handle https
*Varnish cache with persistant file storage to handle caching of dynamicly constructed content (resized images ...) and rewrite of GETs to underlaying systems.
*Elasticsearch for metadata search
*Nginx (with relevant modules) as basic webserver and media server
*IIPImage for zoomable images
*YouTube for video
*Vimeo for video
*Flickr for images
