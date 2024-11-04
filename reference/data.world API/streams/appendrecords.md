---
title: Append record(s)
excerpt: >-
  Append JSON data to a stream associated with a dataset. 


  data.world streams are append-only by default. Alternatively, if a primary key
  is specified (see: `POST:/streams/{owner}/{id}/{streamId}/schema`), data.world
  will replace records with the same primary key value.


  **Streams don't need to be created before you can append data to them**. They
  will be created on-demand, when the first record is appended or by defining
  its schema.


  Multiple records can be appended at once by using JSON-L
  (`application/json-l`) as the request content type.


  **IMPORTANT**


  Data uploaded to a dataset via a stream is not immediatelly processed.
  Instead, it is processed automatically in accordance with the dataset settings
  (default: daily) or as a result of calling `POST:/datasets/{owner}/{id}/sync`.


  Once processed, the contents of a stream will appear as part of the respective
  dataset as a `.jsonl` file (e.g. `my-stream` will produce a file named
  `my-stream.jsonl`).
api:
  file: data-world.json
  operationId: appendRecords
hidden: false
---