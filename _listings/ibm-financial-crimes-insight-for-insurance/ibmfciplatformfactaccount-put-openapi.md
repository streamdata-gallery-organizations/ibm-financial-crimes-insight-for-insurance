---
swagger: "2.0"
x-collection-name: IBM Financial Crimes Insight for Insurance
x-complete: 0
info:
  title: IBM Financial Crimes Insight for Insurance API Insert account data into the
    database
  description: This method is used to insert account data into the database.  The
    XML schema is defined in the ACCOUNT.XSD file.
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
  /ibm/fci/platform/external_alert/analysis_result:
    post:
      summary: Submit assessments from monitored analytics
      description: This method is used to submit analysis results from monitored analysis
      operationId: postExternalAnalyticResult
      x-api-path-slug: ibmfciplatformexternal-alertanalysis-result-post
      parameters:
      - in: body
        name: AnalysisAssessedResults
        description: An XML object corresponding to the AnalysisAssessedResults
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      responses:
        200:
          description: OK
      tags:
      - Submit
      - Assessments
      - From
      - Monitored
      - Analytics
  /ibm/fci/platform/token_service/token:
    get:
      summary: Obtain security token for REST execution
      description: In addition to a username and password required to execute a REST
        service, the platform supports enhanced cross site scripting detection and
        requires a service token for REST API execution.  REST services will need
        to supply the token as both cookie and header in a REST request.
      operationId: getServiceToken
      x-api-path-slug: ibmfciplatformtoken-servicetoken-get
      parameters:
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      responses:
        200:
          description: OK
      tags:
      - Obtain
      - Security
      - TokenREST
      - Execution
  /ibm/fci/platform/fact/account:
    put:
      summary: Insert account data into the database
      description: This method is used to insert account data into the database.  The
        XML schema is defined in the ACCOUNT.XSD file.
      operationId: putAccount
      x-api-path-slug: ibmfciplatformfactaccount-put
      parameters:
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      responses:
        200:
          description: OK
      tags:
      - Insert
      - Account
      - Data
      - Into
      - Database
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