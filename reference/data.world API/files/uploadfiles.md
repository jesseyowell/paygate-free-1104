---
title: Upload files
excerpt: >-
  Upload multiple files at once to a dataset.


  This endpoint expects requests of type `multipart/form-data` and you can
  include one or more parts named `file`, each containing a different file to be
  uploaded.


  For example, assuming that you want to upload two local files named
  `file1.csv` and `file2.csv` to a hypothetical dataset
  `https://data.world/awesome-user/awesome-dataset`, this is what the cURL
  command would look like.


  ```bash

  curl \
    -H "Authorization: Bearer <YOUR_API_TOKEN>" \
    -F "file=@file1.csv" \
    -F "file=@file2.csv" \
    https://api.data.world/v0/uploads/awesome-user/awesome-dataset/files
  ```


  Swagger clients may limit this method of upload to one file at a time. Other
  HTTP clients capable of making multipart/form-data requests can be used to
  upload multiple files in a single request.
api:
  file: data-world.json
  operationId: uploadFiles
hidden: false
---