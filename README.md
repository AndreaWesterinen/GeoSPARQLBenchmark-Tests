# GeoSPARQL Compliance Benchmark Tests

This repository holds test details forked from the _GeoSPARQL Compliance Benchmark_ at https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark. The original repository holds far more tests and is run using the HOBBIT Platform. This subset is used with the [modified Tests for Triplestore (TFT) platform](https://github.com/AndreaWesterinen/TFT).

The benchmark tests in this repository evaluate the GeoSPARQL compliance of RDF storage systems related to the Core, basic geometry, simple features and query rewrite aspects of the [OGC GeoSPARQL standard](https://www.ogc.org/standards/geosparql). They cover requirements #1-4, 7-14, 19, 22 and 28 of the standard, and represent the capabilities relevant to Wikidata.

For reference, the data, queries and results from the src/main/resources directory of the original benchmark are reorganized in the geosparql directory below. Instead of having gsb_queries, _dataset and _answers directories to separate the files, the queries and answers are grouped together within the Core, Topology, Geometry Extension, Geometry Topology Extension and Query Rewrite (core, top, geoext, gtop and qrw) folders. In addition, only the dataset.rdf file is used and is also included in each of the folders.

## Mapping Requirements to Queries

The specific requirments and queries used in this repository are:

| Req. | Set of corresponding queries | Description
| :--: | :--- | :--- 
| <tr><th colspan="3">Core component (CORE)</th></tr>
| R1 | [query-r01.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/core/query-r01.rq) | Selecting the first triple where geometry A is the subject
| R2 | [query-r02.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/core/query-r02.rq) | Selecting the first entity of type [geo:SpatialObject](http://www.opengis.net/ont/geosparql#SpatialObject)
| R3 | [query-r03.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/core/query-r03.rq) | Selecting the first entity of type [geo:Feature](http://www.opengis.net/ont/geosparql#Feature)
| <tr><th colspan="3">Geometry extension (GEOEXT)</th></tr>
| R7 | [query-r07.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r07.rq) | Selecting all entities of type [geo:Geometry](http://www.opengis.net/ont/geosparql#Geometry)
| R8 | [query-r08-1.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r08-1.rq), [query-r08-2.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r08-2.rq) | Selecting the value of geometry A denoted by the properties  [geo:hasGeometry](http://www.opengis.net/ont/geosparql#hasGeometry) and [geo:hasDefaultGeometry](http://www.opengis.net/ont/geosparql#hasDefaultGeometry)
| R9 | [query-r09-1.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r09-1.rq), [query-r09-2.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r09-2.rq),  [query-r09-3.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r09-3.rq), [query-r09-4.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r09-4.rq), <br /> [query-r09-5.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r09-5.rq), [query-r09-6.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r09-6.rq) | Selecting of the value of geometry A denoted by the properties  [geo:dimension](http://www.opengis.net/ont/geosparql#dimension), [geo:coordinateDimension](http://www.opengis.net/ont/geosparql#coordinateDimension), [geo:spatialDimension](http://www.opengis.net/ont/geosparql#spatialDimension),  [geo:isEmpty](http://www.opengis.net/ont/geosparql#isEmpty), [geo:isSimple](http://www.opengis.net/ont/geosparql#isSimple) and [geo:hasSerialization](http://www.opengis.net/ont/geosparql#hasSerialization)| 
| R10 | [query-r10.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r10.rq) | Checking the datatype of a correctly defined WKT literal from the dataset
| R11 | [query-r11.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r11.rq) | Checking the equality of two geometries from the dataset
| R12 | [query-r12.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r12.rq) | Checking the system interprets the axis order within a point geometry  according to the spatial reference system being used
| R13 | [query-r13-1.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r13-1.rq), [query-r13-2.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r13-2.rq) | Checking if an empty RDFS Literal of type [geo:wktLiteral](http://www.opengis.net/ont/geosparql#wktLiteral) is interpreted as  an empty geometry
| R14 | [query-r14.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r14.rq) | Checking the [geo:asWKT](http://www.opengis.net/ont/geosparql#asWKT) value of geometry A against the expected  literal value
| R19 | [query-r19-1-1.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r19-1-1.rq), [query-r19-2-1.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r19-2-1.rq), [query-r19-3-1.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r19-3-1.rq), [query-r19-4-1.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r19-4-1.rq), [query-r19-5-1.rq]https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r19-5-1.rq), [query-r19-6-1.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r19-6-1.rq), [query-r19-7-1.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r19-7-1.rq), [query-r19-8-1.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/geoext/query-r19-8-1.rq) | Checking support of the geospatial functions [geof:distance](http://www.opengis.net/def/function/geosparql/distance), [geof:buffer](http://www.opengis.net/def/function/geosparql/buffer),  [geof:convexHull](http://www.opengis.net/def/function/geosparql/convexHull), [geof:intersection](http://www.opengis.net/def/function/geosparql/intersection), [geof:union](http://www.opengis.net/def/function/geosparql/union), [geof:difference](http://www.opengis.net/def/function/geosparql/difference),  [geof:symDifference](http://www.opengis.net/def/function/geosparql/symDifference), [geof:envelope](http://www.opengis.net/def/function/geosparql/envelope) and [geof:boundary](http://www.opengis.net/def/function/geosparql/boundary), for the WKT geometry
| <tr><th colspan="3">Geometry topology extension (GTOP)</th></tr>
| R22 | [query-r22-1-1.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/gtop/query-r22-1-1.rq), [query-r22-2-1.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/gtop/query-r22-2-1.rq), [query-r22-3-1.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/gtop/query-r22-3-1.rq), [query-r22-4-1.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/gtop/query-r22-4-1.rq), [query-r22-5-1.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/gtop/query-r22-5-1.rq), [query-r22-6-1.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/gtop/query-r22-6-1.rq), [query-r22-7-1.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/gtop/query-r22-7-1.rq), [query-r22-8-1.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/gtop/query-r22-8-1.rq) | Checking support of the geospatial functions [geof:sfEquals](http://www.opengis.net/def/function/geosparql/sfEquals), [geof:sfDisjoint](http://www.opengis.net/def/function/geosparql/sfDisjoint),  [geof:sfIntersects](http://www.opengis.net/def/function/geosparql/sfIntersects), [geof:sfTouches](http://www.opengis.net/def/function/geosparql/sfTouches), [geof:sfCrosses](http://www.opengis.net/def/function/geosparql/sfCrosses), [geof:sfWithin](http://www.opengis.net/def/function/geosparql/sfWithin), [geof:sfContains](http://www.opengis.net/def/function/geosparql/sfContains)  and [geof:sfOverlaps](http://www.opengis.net/def/function/geosparql/sfOverlaps) for the WKT geometry
| <tr><th colspan="3">Query Rewriting of the Simple Features (QRW)</th></tr>
| R28 | [query-r28-1.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/qrw/query-r28-1.rq), [query-r28-2.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/qrw/query-r28-2.rq), [query-r28-3.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/qrw/query-r28-3.rq), [query-r28-4.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/qrw/query-r28-4.rq), [query-r28-5.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/qrw/query-r28-5.rq), [query-r28-6.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/qrw/query-r28-6.rq), [query-r28-7.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/qrw/query-r28-7.rq), [query-r28-8.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/qrw/query-r28-8.rq) | Testing the properties, geo:sfEquals, geo:sfDisjoint, geo:sfIntersects, geo:sfTouches, geo:sfCrosses, geo:sfWithin, geo:sfContains and geo:sfOverlaps, between features and geometries
| <tr><th colspan="3">Topology vocabulary extension (TOP)</th></tr>
| R4 | [query-r04-1.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/top/query-r04-1.rq), [query-r04-2.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/top/query-r04-2.rq),  [query-r04-3.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/top/query-r04-3.rq), [query-r04-4.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/top/query-r04-4.rq), <br /> [query-r04-5.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/top/query-r04-5.rq), [query-r04-6.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/top/query-r04-6.rq),  [query-r04-7.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/top/query-r04-7.rq), [query-r04-8.rq](https://github.com/AndreaWesterinen/GeoSPARQLBenchmark/tree/master/geosparql/top/query-r04-8.rq) | Testing the properties, [geo:sfEquals](http://www.opengis.net/ont/geosparql#sfEquals), [geo:sfDisjoint](http://www.opengis.net/ont/geosparql#sfDisjoint), [geo:sfIntersects](http://www.opengis.net/ont/geosparql#sfIntersects),  [geo:sfTouches](http://www.opengis.net/ont/geosparql#sfTouches), [geo:sfCrosses](http://www.opengis.net/ont/geosparql#sfCrosses), [geo:sfWithin](http://www.opengis.net/ont/geosparql#sfWithin), [geo:sfContains](http://www.opengis.net/ont/geosparql#sfContains) and  [geo:sfOverlaps](http://www.opengis.net/ont/geosparql#sfOverlaps)
 
## Acknowledgement

The original benchmark was developed as part of the [HOBBIT](https://project-hobbit.eu) and [SAGE](https://sage.cs.uni-paderborn.de/sage/) research projects.
