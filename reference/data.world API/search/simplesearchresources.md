---
title: Simple search on resources
excerpt: >-
  Simple search is a light weight API implementation exposing similar search
  capabilities as our main platform search UI.


  By default, the search response will return mixed result types including
  metadata resources, datasets, projects, queries, insights, tables, and
  comments.


  A free-text search term is required. Simple search does not support complex
  keyword or logical operator grammar.

  Light weight filters for resource owner and resource category are supported.
  You may optionally specify the includeCommunityResults param to query for
  resources in the data.world open data community.
api:
  file: data-world.json
  operationId: simpleSearchResources
hidden: false
---