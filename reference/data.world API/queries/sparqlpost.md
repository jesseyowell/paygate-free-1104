---
title: SPARQL query
excerpt: >-
  Execute a SPARQL query against a dataset or data project.


  SPARQL results are available in a variety of formats. By default,
  `application/sparql-results+json` will be returned. Set the `Accept` header to
  one of the following values in accordance with your preference:


  - `application/sparql-results+xml`

  - `application/sparql-results+json`

  - `application/rdf+json`

  - `application/rdf+xml`

  - `text/csv`

  - `text/tab-separated-values`

  - `text/turtle`


  New to SPARQL? Check out data.world's [SPARQL
  tutorial](https://docs.data.world/tutorials/sparql/).
api:
  file: data-world.json
  operationId: sparqlPost
hidden: false
---