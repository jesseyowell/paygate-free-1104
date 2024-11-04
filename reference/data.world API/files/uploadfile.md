---
title: Upload a file
excerpt: >-
  Upload one file at a time to a dataset.


  This endpoint expects requests of type `application/octet-stream`.


  For example, assuming that you want to upload a local file named `file1.csv`
  to a hypothetical dataset `https://data.world/awesome-user/awesome-dataset`
  and choose its name on data.world to be `better-name.csv`, this is what the
  cURL command would look like.


  ```bash

  curl \
    -H "Authorization: Bearer <YOUR_API_TOKEN>" \
    -X PUT -H "Content-Type: application/octet-stream" \
    --data-binary @file1.csv \
    https://api.data.world/v0/uploads/awesome-user/awesome-dataset/files/better-name.csv
  ```


  This method of upload is typically not supported by Swagger clients. Other
  HTTP clients can be used to supply the contents of the file directly in the
  body of the request.
api:
  file: data-world.json
  operationId: uploadFile
hidden: false
---