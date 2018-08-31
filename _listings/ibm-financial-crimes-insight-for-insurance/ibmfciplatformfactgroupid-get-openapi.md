---
swagger: "2.0"
x-collection-name: IBM Financial Crimes Insight for Insurance
x-complete: 0
info:
  title: IBM Financial Crimes Insight for Insurance API Retrieve group data from the
    database, for the specific group id
  description: This method is used to retrieve specific group data from the database
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
  /ibm/fci/platform/fact/entity/{id}:
    get:
      summary: Get the data for the resolved entity id.
      description: Using the provided party id, obtain the entity id
      operationId: getResolvedEntityById
      x-api-path-slug: ibmfciplatformfactentityid-get
      parameters:
      - in: body
        name: Entity
        description: A JSON structure that provide the details of an entity
        schema:
          $ref: '#/definitions/holder'
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
      - Datathe
      - Resolved
      - Entity
      - Id
  /ibm/fci/platform/fact/entitysearch:
    post:
      summary: Search for objects that match the search terms specified.
      description: 'Search for objects that match the search terms specified.  The
        searchType refers to the type of object being searched for. Valid values include:
        Folio,Account,Event,Group,PhysicalObject,Party,Transaction,Any. Note that
        paging and ordering is not supported for type Any.  The parameter globalsearch
        represents a global search string with support for the * wildcard.  The propertysearch
        fields are a list of searches for matching on specified fields of an object.'
      operationId: entitySearch
      x-api-path-slug: ibmfciplatformfactentitysearch-post
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
      responses:
        200:
          description: OK
      tags:
      - Searchobjects
      - That
      - Match
      - Search
      - Terms
      - Specified
  /ibm/fci/platform/fact/entity/relatedparties/{systemId}/{remoteReference}:
    get:
      summary: This method is used to retrieve the set of explicitly related parties
        and implicitly related entities for the supplied externally sourced reference
        party
      description: |-
        A data source must be configured in the appropriate server.xml to use ISII. Ensure that the following has been included:

        &lt;dataSource beginTranForResultSetScrollingAPIs="false" id="ISIIDB" isolationLevel="TRANSACTION_READ_COMMITTED" jndiName="jdbc/isii"&gt;

        &lt;jdbcDriver javax.sql.DataSource="com.ibm.db2.jcc.DB2XADataSource" libraryRef="DB2_LIB"/&gt;

        &lt;properties.db2.jcc databaseName="ISII" password="${isii_db_pass}" portNumber="${isii_db_port}" serverName="${isii_host}" user="${isii_db_user}"/&gt;

        &lt;connectionManager connectionTimeout="60s" maxIdleTime="3m" maxPoolSize="200" minPoolSize="0"/&gt;

        &lt;/dataSource&gt;

        Where password, portNumber, serverName, and user values are replaced with the appropriate properties or environment variables for your configuration.
      operationId: getRelatedObjects
      x-api-path-slug: ibmfciplatformfactentityrelatedpartiessystemidremotereference-get
      parameters:
      - in: query
        name: minRelatedScore
        description: Minimum matching score for implicit relationships
      - in: path
        name: remoteReference
        description: Remote reference object key
      - in: path
        name: systemId
        description: Remote reference system ID
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Retrieve
      - Set
      - Of
      - Explicitly
      - Related
      - Parties
      - Implicitly
      - Related
      - Entitiesthe
      - Supplied
      - Externally
      - Sourced
      - Reference
      - Party
  /ibm/fci/platform/fact/event:
    put:
      summary: Insert event data into the database
      description: This method is used to insert event data into the database.  The
        XML schema is defined in the EVENT.XSD file.
      operationId: putEvent
      x-api-path-slug: ibmfciplatformfactevent-put
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
      responses:
        200:
          description: OK
      tags:
      - Insert
      - Event
      - Data
      - Into
      - Database
  /ibm/fci/platform/fact/event/{id}:
    get:
      summary: Retrieve event data from the database, for the id
      description: This method is used to retrieve event data from the database
      operationId: getEvent
      x-api-path-slug: ibmfciplatformfacteventid-get
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
      - Event
      - Data
      - From
      - Database
      - The
      - Id
  /ibm/fci/platform/fact/group:
    put:
      summary: Insert group data into the database
      description: This method is used to insert group data into the database.  The
        XML schema is defined in the GROUP.XSD file.
      operationId: putGroup
      x-api-path-slug: ibmfciplatformfactgroup-put
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
      responses:
        200:
          description: OK
      tags:
      - Insert
      - Group
      - Data
      - Into
      - Database
  /ibm/fci/platform/fact/group/{id}:
    get:
      summary: Retrieve group data from the database, for the specific group id
      description: This method is used to retrieve specific group data from the database
      operationId: getGroup
      x-api-path-slug: ibmfciplatformfactgroupid-get
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
      - Group
      - Data
      - From
      - Database
      - The
      - Specific
      - Group
      - Id
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