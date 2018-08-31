---
swagger: "2.0"
x-collection-name: IBM Financial Crimes Insight for Insurance
x-complete: 0
info:
  title: IBM Financial Crimes Insight for Insurance API Get a list of resolved objects
    from resolved entities for a given object.
  description: Get a list of resolved objects from resolved entities for a given object.
    Using the provided object ID, produce a list of all objects of the same business
    object type that have been determined to be 'matches'.
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
  /ibm/fci/platform/fact/account/{id}:
    get:
      summary: Retrieve account data from the database, for the id
      description: This method is used to retrieve account data from the database
      operationId: getAccount
      x-api-path-slug: ibmfciplatformfactaccountid-get
      parameters:
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Account
      - Data
      - From
      - Database
      - The
      - Id
  /ibm/fci/platform/fact/{type}/{remoteSystem}/{remoteKey}/assessments]:
    get:
      summary: Return the existing assessments for the object specified
      description: This service is used to return the existing assessments for the
        object specified.
      operationId: requestAssessmentValue
      x-api-path-slug: ibmfciplatformfacttyperemotesystemremotekeyassessments-get
      parameters:
      - in: query
        name: context
        description: The fraud context for which to return assessements
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: path
        name: remoteKey
        description: The combination of remoteSystem and remoteKey uniquely defines
          an object
      - in: path
        name: remoteSystem
        description: The combination of remoteSystem and remoteKey uniquely defines
          an object
      - in: path
        name: type
        description: Type of object; party, account, transaction, event, or other
          defined object type
      responses:
        200:
          description: OK
      tags:
      - Return
      - Existing
      - Assessmentsthe
      - Object
      - Specified
  /ibm/fci/platform/fact/entity/{remote_system_id}/{external_remote_reference}:
    get:
      summary: Retrieve set of identities considered to be the same entity
      description: This method is used to retrieve the set of individuals (or organizations)
        that are considered the same as the provided party reference
      operationId: getResolvedEntityByRef
      x-api-path-slug: ibmfciplatformfactentityremote-system-idexternal-remote-reference-get
      parameters:
      - in: path
        name: external_remote_reference
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: path
        name: remote_system_id
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Set
      - Of
      - Identities
      - Considered
      - To
      - Be
      - Same
      - Entity
  /ibm/fci/platform/fact/match:
    get:
      summary: Determine if one object is a match to the other.
      description: Using the provided objects, determine if one is a 'match' of the
        other
      operationId: getMatchedObject
      x-api-path-slug: ibmfciplatformfactmatch-get
      parameters:
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: query
        name: objectId1
        description: Object id of first object
      - in: query
        name: objectId2
        description: Object id of second object
      - in: query
        name: objectStereotype
        description: stereotype of the objects being compared
      - in: query
        name: updateResolvedEntities
        description: Boolean to indicate whether or not to record relationship
      responses:
        200:
          description: OK
      tags:
      - Determine
      - If
      - Object
      - Is
      - Match
      - To
      - Other
  /ibm/fci/platform/fact/entity/match:
    get:
      summary: Get a list of resolved objects from resolved entities for a given object.
      description: Get a list of resolved objects from resolved entities for a given
        object. Using the provided object ID, produce a list of all objects of the
        same business object type that have been determined to be 'matches'.
      operationId: getMatchedEntity
      x-api-path-slug: ibmfciplatformfactentitymatch-get
      parameters:
      - in: query
        name: count
        description: Number of objects to return; all if not included
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: query
        name: id
        description: Object id of the object
      - in: query
        name: logicalType
        description: Metadata element ID for a business object
      - in: query
        name: returnFlag
        description: Default value == 2
      - in: query
        name: threshold
        description: Minimum matching score to include a resolved entity; defaults
          to system property if not supplied
      - in: query
        name: type
        description: Stereotype for object
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Resolved
      - Objects
      - From
      - Resolved
      - Entitiesa
      - Given
      - Object
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