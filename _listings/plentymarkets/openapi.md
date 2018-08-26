---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/system/cloud/metrics:
    get:
      summary: Get the cloud metrics for this system
      description: Get the cloud metrics for this system.
      operationId: getRestSystemCloudMetrics
      x-api-path-slug: restsystemcloudmetrics-get
      responses:
        2:
          description: Successful response
        200:
          description: OK
      tags:
      - Cloud
      - Metricsthis
      - System
---