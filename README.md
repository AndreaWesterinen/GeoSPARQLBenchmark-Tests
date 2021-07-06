# GeoSPARQL Compliance Benchmark

This is the GeoSPARQL Compliance Benchmark, integrated into the [HOBBIT Platform](https://github.com/hobbit-project/platform).

The GeoSPARQL Compliance Benchmark aims to evaluate the GeoSPARQL compliance of RDF storage systems. The benchmark uses
206 SPARQL queries to test the extent to which the benchmarked system supports the 30 requirements defined in the [GeoSPARQL standard](https://www.ogc.org/standards/geosparql).

As a result, the benchmark provides two metrics:
 * **Correct answers**: The number of correct answers out of all GeoSPARQL queries, i.e. tests.
 * **GeoSPARQL compliance percentage**: The percentage of compliance with the requirements of the GeoSPARQL standard.

## Results

You can find a set of results from the [latest experiments on the hosted instance of the HOBBIT Platform](https://master.project-hobbit.eu/experiments/1612476122572,1612477003063,1612476116049,1612477500164,1612661614510,1612637531673,1612828110551,1612477849872)
(log in as Guest). [last update: 09.02.2021]

If you want your RDF triplestore tested, you can [add it as a system to the HOBBIT Platform](https://hobbit-project.github.io/system_integration.html),
and then [run an experiment](https://hobbit-project.github.io/benchmarking.html) using the [hosted instance of the HOBBIT Platform](https://hobbit-project.github.io/master.html).

## Publications

 * Milos Jovanovik, Timo Homburg, Mirko Spasić. "[Software for the GeoSPARQL Compliance Benchmark](https://doi.org/10.1016/j.simpa.2021.100071)". Software Impacts 8:100071, 2021.
 * (preprint) Milos Jovanovik, Timo Homburg, Mirko Spasić. "[A GeoSPARQL Compliance Benchmark](https://arxiv.org/abs/2102.06139)". arXiv:2102.06139.

## Mapping Requirements to Queries

Requirement | Queries | Description
--- | --- | --- 
R1 | [query-r01.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r01.rq) | Selection of the first triple where geometry A is the subject (ordered by the predicates and the objects)
R2 | [query-r02.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r02.rq) | 
R3 | [query-r03.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r03.rq) | 
R4 | [query-r04-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r04-1.rq), [query-r04-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r04-2.rq), [query-r04-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r04-3.rq), [query-r04-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r04-4.rq), <br /> [query-r04-5.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r04-5.rq), [query-r04-6.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r04-6.rq), [query-r04-7.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r04-7.rq), [query-r04-8.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r04-8.rq) | 
R5 | [query-r05-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r05-1.rq), [query-r05-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r05-2.rq), [query-r05-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r05-3.rq), [query-r05-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r05-4.rq), <br /> [query-r05-5.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r05-5.rq), [query-r05-6.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r05-6.rq), [query-r05-7.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r05-7.rq), [query-r05-8.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r05-8.rq) | 
R6 | [query-r06-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r06-1.rq), [query-r06-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r06-2.rq), [query-r06-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r06-3.rq), [query-r06-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r06-4.rq), <br /> [query-r06-5.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r06-5.rq), [query-r06-6.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r06-6.rq), [query-r06-7.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r06-7.rq), [query-r06-8.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r06-8.rq) | 
R7 | [query-r07.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r07.rq) | 
R8 | [query-r08-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r08-1.rq), [query-r08-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r08-2.rq) | 
R9 | [query-r09-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r09-1.rq), [query-r09-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r09-2.rq), [query-r09-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r09-3.rq), [query-r09-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r09-4.rq), <br /> [query-r09-5.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r09-5.rq), [query-r09-6.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r09-6.rq) | 
R10 | [query-r10.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r10.rq) | 
R11 | [query-r11.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r11.rq) | 
R12 | [query-r12.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r12.rq) | 
R13 | [query-r13-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r13-1.rq), [query-r13-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r13-2.rq) | 
R14 | [query-r14.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r14.rq) | 
R15 | [query-r15.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r15.rq) | 
R16 | [query-r16-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r16-1.rq), [query-r16-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r16-2.rq) | 
R17 | --- | 
R18 | [query-r18.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r18.rq) | 
R19 | [query-r19-1-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-1-1.rq), [query-r19-1-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-1-2.rq), [query-r19-1-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-1-3.rq), [query-r19-1-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-1-4.rq), <br /> [query-r19-2-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-2-1.rq), [query-r19-2-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-2-2.rq), <br /> [query-r19-3-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-3-1.rq), [query-r19-3-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-3-2.rq), <br /> [query-r19-4-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-4-1.rq), [query-r19-4-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-4-2.rq), [query-r19-4-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-4-3.rq), [query-r19-4-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-4-4.rq), <br /> [query-r19-5-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-5-1.rq), [query-r19-5-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-5-2.rq), [query-r19-5-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-5-3.rq), [query-r19-5-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-5-4.rq), <br /> [query-r19-6-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-6-1.rq), [query-r19-6-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-6-2.rq), [query-r19-6-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-6-3.rq), [query-r19-6-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-6-4.rq), <br /> [query-r19-7-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-7-1.rq), [query-r19-7-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-7-2.rq), [query-r19-7-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-7-3.rq), [query-r19-7-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-7-4.rq), <br /> [query-r19-8-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-8-1.rq), [query-r19-8-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-8-2.rq), <br /> [query-r19-9-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-9-1.rq), [query-r19-9-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r19-9-2.rq) | 
R20 | [query-r20-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r20-1.rq), [query-r20-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r20-2.rq) |
R21 | [query-r21-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r21-1.rq), [query-r21-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r21-2.rq), [query-r21-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r21-3.rq), [query-r21-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r21-4.rq) | 
R22 | [query-r22-1-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-1-1.rq), [query-r22-1-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-1-2.rq), [query-r22-1-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-1-3.rq), [query-r22-1-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-1-4.rq), <br /> [query-r22-2-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-2-1.rq), [query-r22-2-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-2-2.rq), [query-r22-2-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-2-3.rq), [query-r22-2-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-2-4.rq), <br /> [query-r22-3-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-3-1.rq), [query-r22-3-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-3-2.rq), [query-r22-3-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-3-3.rq), [query-r22-3-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-3-4.rq), <br /> [query-r22-4-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-4-1.rq), [query-r22-4-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-4-2.rq), [query-r22-4-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-4-3.rq), [query-r22-4-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-4-4.rq), <br /> [query-r22-5-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-5-1.rq), [query-r22-5-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-5-2.rq), [query-r22-5-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-5-3.rq), [query-r22-5-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-5-4.rq), <br /> [query-r22-6-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-6-1.rq), [query-r22-6-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-6-2.rq), [query-r22-6-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-6-3.rq), [query-r22-6-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-6-4.rq), <br /> [query-r22-7-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-7-1.rq), [query-r22-7-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-7-2.rq), [query-r22-7-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-7-3.rq), [query-r22-7-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-7-4.rq), <br /> [query-r22-8-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-8-1.rq), [query-r22-8-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-8-2.rq), [query-r22-8-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-8-3.rq), [query-r22-8-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r22-8-4.rq) | 
R23 | [query-r23-1-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-1-1.rq), [query-r23-1-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-1-2.rq), [query-r23-1-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-1-3.rq), [query-r23-1-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-1-4.rq), <br /> [query-r23-2-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-2-1.rq), [query-r23-2-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-2-2.rq), [query-r23-2-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-2-3.rq), [query-r23-2-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-2-4.rq), <br /> [query-r23-3-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-3-1.rq), [query-r23-3-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-3-2.rq), [query-r23-3-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-3-3.rq), [query-r23-3-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-3-4.rq), <br /> [query-r23-4-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-4-1.rq), [query-r23-4-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-4-2.rq), [query-r23-4-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-4-3.rq), [query-r23-4-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-4-4.rq), <br /> [query-r23-5-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-5-1.rq), [query-r23-5-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-5-2.rq), [query-r23-5-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-5-3.rq), [query-r23-5-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-5-4.rq), <br /> [query-r23-6-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-6-1.rq), [query-r23-6-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-6-2.rq), [query-r23-6-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-6-3.rq), [query-r23-6-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-6-4.rq), <br /> [query-r23-7-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-7-1.rq), [query-r23-7-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-7-2.rq), [query-r23-7-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-7-3.rq), [query-r23-7-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-7-4.rq), <br /> [query-r23-8-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-8-1.rq), [query-r23-8-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-8-2.rq), [query-r23-8-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-8-3.rq), [query-r23-8-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r23-8-4.rq) | 
R24 | [query-r24-1-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-1-1.rq), [query-r24-1-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-1-2.rq), [query-r24-1-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-1-3.rq), [query-r24-1-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-1-4.rq), <br /> [query-r24-2-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-2-1.rq), [query-r24-2-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-2-2.rq), [query-r24-2-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-2-3.rq), [query-r24-2-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-2-4.rq), <br /> [query-r24-3-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-3-1.rq), [query-r24-3-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-3-2.rq), [query-r24-3-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-3-3.rq), [query-r24-3-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-3-4.rq), <br /> [query-r24-4-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-4-1.rq), [query-r24-4-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-4-2.rq), [query-r24-4-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-4-3.rq), [query-r24-4-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-4-4.rq), <br /> [query-r24-5-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-5-1.rq), [query-r24-5-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-5-2.rq), [query-r24-5-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-5-3.rq), [query-r24-5-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-5-4.rq), <br /> [query-r24-6-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-6-1.rq), [query-r24-6-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-6-2.rq), [query-r24-6-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-6-3.rq), [query-r24-6-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-6-4.rq), <br /> [query-r24-7-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-7-1.rq), [query-r24-7-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-7-2.rq), [query-r24-7-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-7-3.rq), [query-r24-7-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-7-4.rq), <br /> [query-r24-8-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-8-1.rq), [query-r24-8-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-8-2.rq), [query-r24-8-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-8-3.rq), [query-r24-8-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r24-8-4.rq) | 
R25 | [query-r25-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r25-1.rq), [query-r25-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r25-2.rq), [query-r25-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r25-3.rq) | 
R26 | [query-r26-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r26-1.rq), [query-r26-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r26-2.rq) | 
R27 | [query-r27.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r27.rq) | 
R28 | [query-r28-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r28-1.rq), [query-r28-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r28-2.rq), [query-r28-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r28-3.rq), [query-r28-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r28-4.rq), <br /> [query-r28-5.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r28-5.rq), [query-r28-6.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r28-6.rq), [query-r28-7.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r28-7.rq), [query-r28-8.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r28-8.rq) | 
R29 | [query-r29-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r29-1.rq), [query-r29-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r29-2.rq), [query-r29-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r29-3.rq), [query-r29-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r29-4.rq), <br /> [query-r29-5.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r29-5.rq), [query-r29-6.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r29-6.rq), [query-r29-7.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r29-7.rq), [query-r29-8.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r29-8.rq) | 
R30 | [query-r30-1.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r30-1.rq), [query-r30-2.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r30-2.rq), [query-r30-3.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r30-3.rq), [query-r30-4.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r30-4.rq), <br /> [query-r30-5.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r30-5.rq), [query-r30-6.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r30-6.rq), [query-r30-7.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r30-7.rq), [query-r30-8.rq](https://github.com/OpenLinkSoftware/GeoSPARQLBenchmark/blob/master/src/main/resources/gsb_queries/query-r30-8.rq) | 

## Acknowledgement

The benchmark has been developed as part of the [HOBBIT](https://project-hobbit.eu) and [SAGE](https://sage.cs.uni-paderborn.de/sage/) research projects.
