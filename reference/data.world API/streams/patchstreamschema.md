---
title: Set / Update stream schema
excerpt: >-
  Set or update a stream's schema.


  The schema of a stream defines its primary key(s) and sort/sequence field. 


  data.world streams are append-only by default. Alternatively, if a primary key
  is specified, data.world will replace records with the same primary key value.
  data.world will sort records by sequence field value and will discard all but
  the last record appended for each given primary key value.


  The `updateMethod` parameter specifies how data.world should handle existing
  records when schema is updated. Currently, the only `updateMethod` supported
  is `TRUNCATED`. data.world will discard all records when the schema is
  updated.
api:
  file: data-world.json
  operationId: patchStreamSchema
hidden: false
---