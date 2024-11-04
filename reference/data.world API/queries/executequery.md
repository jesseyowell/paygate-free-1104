---
title: Execute a saved query
excerpt: >-
  Execute a saved query.


  SQL results are available in a variety of formats. By default,
  `application/json` will be returned. Set the `Accept` header to one of the
  following values in accordance with your preference:


  * `text/csv`

  * `application/json`

  * `application/json-l`

  * `application/x-ndjson`


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
api:
  file: data-world.json
  operationId: executeQuery
hidden: false
---