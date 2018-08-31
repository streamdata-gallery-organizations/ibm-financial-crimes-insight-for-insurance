---
swagger: "2.0"
x-collection-name: IBM Financial Crimes Insight for Insurance
x-complete: 0
info:
  title: IBM Financial Crimes Insight for Insurance API Request a managed analysis
    to run
  description: This service can be used to initiate a managed analysis
  version: 1.0.0
host: fcihost.ibm.com:9443
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ibm/fci/platform/data_access/analysis_request:
    post:
      summary: Request a managed analysis to run
      description: This service can be used to initiate a managed analysis
      operationId: startAnalysis
      x-api-path-slug: ibmfciplatformdata-accessanalysis-request-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: query
        name: waitTime
        description: wait for NN seconds, and if no response continue
      responses:
        200:
          description: OK
      tags:
      - Request
      - Managed
      - Analysis
      - To
      - Run
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