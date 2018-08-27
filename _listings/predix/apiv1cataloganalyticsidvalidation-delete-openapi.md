---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Analytics Framework Undeploy test analytics.
  version: 1.0.0
  description: This operation un-deploys the analytic app from the Cloud Foundry environment
    only if the analytic has been validated for testing purposes. This api will not
    un-deploy production analytics.
host: predix-acs.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/catalog/analytics/{id}/deployment:
    post:
      summary: Deploy an analytic with an optional deployment configuration by analytic
        catalog entry id.
      description: This operation FORCE deploys the specified analytic into the Cloud
        Foundry environment with an optional deployment configuration, responds with
        the request id (generated for the request), and the current request status.  The
        force deploy usually takes longer than the standard timeout, so the calling
        process should use the returned request id to monitor the request status and
        to retrieve the deployment results.
      operationId: deployAnalytic
      x-api-path-slug: apiv1cataloganalyticsiddeployment-post
      parameters:
      - in: body
        name: body
        description: deployment configuration
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: analytic catalog entry id
      responses:
        2:
          description: Successful response
      tags:
      - Deploy
      - Analytic
      - Optional
      - Deployment
      - Configuration
      - By
      - Analytic
      - Catalog
      - Entry
      - Id
  /api/v1/catalog/analytics/{id}/validation:
    post:
      summary: Validate an analytic by analytic catalog entry id.
      description: This operation FORCE deploys the specified analytic into the Cloud
        Foundry environment, runs the analytic and responds with the validation request
        id (generated for the request), and the current request status.  The force
        deploy usually takes longer than the standard timeout, so the calling process
        should use the returned validation request id to monitor the request status
        and to retrieve the validation results.
      operationId: validateAnalytic
      x-api-path-slug: apiv1cataloganalyticsidvalidation-post
      parameters:
      - in: body
        name: body
        description: request payload containing analytic input data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: analytic catalog entry id
      - in: query
        name: inputId
        description: test artifact id
      responses:
        200:
          description: OK
      tags:
      - Validate
      - Analytic
      - By
      - Analytic
      - Catalog
      - Entry
      - Id
    delete:
      summary: Undeploy test analytics.
      description: This operation un-deploys the analytic app from the Cloud Foundry
        environment only if the analytic has been validated for testing purposes.
        This api will not un-deploy production analytics.
      operationId: invalidateAnalytic
      x-api-path-slug: apiv1cataloganalyticsidvalidation-delete
      parameters:
      - in: path
        name: id
        description: analytic catalog entry id
      responses:
        2:
          description: Successful response
      tags:
      - Undeploy
      - Test
      - Analytics
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---