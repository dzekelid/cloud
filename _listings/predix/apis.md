---
name: Predix
x-slug: predix
description: Predix (IoT PaaS) helps you develop apps that connect people with industrial
  machines through analytics and data for better business outcomes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
x-kinRank: "7"
x-alexaRank: "264121"
tags: Cloud
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/cloud/master/_listings/predix/apis.md
specificationVersion: "0.14"
apis:
- name: Analytics Catalog - Deploy an analytic with an optional deployment configuration
    by analytic catalog entry id.
  x-api-slug: apiv1cataloganalyticsiddeployment-post
  description: This operation FORCE deploys the specified analytic into the Cloud
    Foundry environment with an optional deployment configuration, responds with the
    request id (generated for the request), and the current request status.  The force
    deploy usually takes longer than the standard timeout, so the calling process
    should use the returned request id to monitor the request status and to retrieve
    the deployment results.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cloud/master/_listings/predix/apiv1cataloganalyticsiddeployment-post-openapi.md
- name: Analytics Catalog - Validate an analytic by analytic catalog entry id.
  x-api-slug: apiv1cataloganalyticsidvalidation-post
  description: This operation FORCE deploys the specified analytic into the Cloud
    Foundry environment, runs the analytic and responds with the validation request
    id (generated for the request), and the current request status.  The force deploy
    usually takes longer than the standard timeout, so the calling process should
    use the returned validation request id to monitor the request status and to retrieve
    the validation results.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cloud/master/_listings/predix/apiv1cataloganalyticsidvalidation-post-openapi.md
- name: Analytics Catalog - Undeploy test analytics.
  x-api-slug: apiv1cataloganalyticsidvalidation-delete
  description: This operation un-deploys the analytic app from the Cloud Foundry environment
    only if the analytic has been validated for testing purposes. This api will not
    un-deploy production analytics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cloud/master/_listings/predix/apiv1cataloganalyticsidvalidation-delete-openapi.md
- name: Analytics Framework - Deploy an analytic with an optional deployment configuration
    by analytic catalog entry id.
  x-api-slug: apiv1cataloganalyticsiddeployment-post
  description: This operation FORCE deploys the specified analytic into the Cloud
    Foundry environment with an optional deployment configuration, responds with the
    request id (generated for the request), and the current request status.  The force
    deploy usually takes longer than the standard timeout, so the calling process
    should use the returned request id to monitor the request status and to retrieve
    the deployment results.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cloud/master/_listings/predix/apiv1cataloganalyticsiddeployment-post-openapi.md
- name: Analytics Framework - Undeploy test analytics.
  x-api-slug: apiv1cataloganalyticsidvalidation-delete
  description: This operation un-deploys the analytic app from the Cloud Foundry environment
    only if the analytic has been validated for testing purposes. This api will not
    un-deploy production analytics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cloud/master/_listings/predix/apiv1cataloganalyticsidvalidation-delete-openapi.md
- name: Analytics Framework - Validate an analytic by analytic catalog entry id.
  x-api-slug: apiv1cataloganalyticsidvalidation-post
  description: This operation FORCE deploys the specified analytic into the Cloud
    Foundry environment, runs the analytic and responds with the validation request
    id (generated for the request), and the current request status.  The force deploy
    usually takes longer than the standard timeout, so the calling process should
    use the returned validation request id to monitor the request status and to retrieve
    the validation results.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/predix-vector-logo.png
  humanURL: https://www.predix.io
  baseURL: https:////
  tags: SaaS, Technology, Enterprise, Internet of Things, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/cloud/master/_listings/predix/apiv1cataloganalyticsidvalidation-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://predicthq.api.gallery.streamdata.io
- type: x-api-stack
  url: http://predix.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/predix
- type: x-documentation
  url: https://docs.predix.io/en-US/platform
- type: x-twitter
  url: https://twitter.com/Predix
- type: x-website
  url: https://www.predix.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---