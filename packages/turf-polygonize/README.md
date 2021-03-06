# @turf/polygonize

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

## polygonize

Polygonizes [(Multi)LineString(s)](https://tools.ietf.org/html/rfc7946#section-3.1.4) into [Polygons](https://tools.ietf.org/html/rfc7946#section-3.1.6).

Implementation of GEOSPolygonize function (`geos::operation::polygonize::Polygonizer`).

Polygonizes a set of lines that represents edges in a planar graph. Edges must be correctly
noded, i.e., they must only meet at their endpoints.

The implementation correctly handles:

-   Dangles: edges which have one or both ends which are not incident on another edge endpoint.
-   Cut Edges (bridges): edges that are connected at both ends but which do not form part of a polygon.

**Parameters**

-   `geoJson` **([FeatureCollection](https://tools.ietf.org/html/rfc7946#section-3.3) \| [Geometry](https://tools.ietf.org/html/rfc7946#section-3.1) \| [Feature](https://tools.ietf.org/html/rfc7946#section-3.2)&lt;([LineString](https://tools.ietf.org/html/rfc7946#section-3.1.4) \| [MultiLineString](https://tools.ietf.org/html/rfc7946#section-3.1.5))>)** Lines in order to polygonize


-   Throws **[Error](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error)** if geoJson is invalid.

Returns **[FeatureCollection](https://tools.ietf.org/html/rfc7946#section-3.3)&lt;[Polygon](https://tools.ietf.org/html/rfc7946#section-3.1.6)>** Polygons created

<!-- This file is automatically generated. Please don't edit it directly:
if you find an error, edit the source file (likely index.js), and re-run
./scripts/generate-readmes in the turf project. -->

---

This module is part of the [Turfjs project](http://turfjs.org/), an open source
module collection dedicated to geographic algorithms. It is maintained in the
[Turfjs/turf](https://github.com/Turfjs/turf) repository, where you can create
PRs and issues.

### Installation

Install this module individually:

```sh
$ npm install @turf/polygonize
```

Or install the Turf module that includes it as a function:

```sh
$ npm install @turf/turf
```
