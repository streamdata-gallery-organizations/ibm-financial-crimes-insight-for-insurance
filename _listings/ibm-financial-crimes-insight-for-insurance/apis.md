---
name: IBM Financial Crimes Insight for Insurance
x-slug: ibm-financial-crimes-insight-for-insurance
description: IBM&reg; Financial Crimes Insight&reg; for Insurance V3.0, formerly known
  as IBM Counter Fraud Management for Insurance, is now being offered as a cloud service
  offering. It helps organizations analyze data to determine the fraud risk of claims,
  medical providers, and other business entities, manage the full investigation lifecycle,
  and report on outcomes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
x-kinRank: "7"
x-alexaRank: ""
tags: IBM Financial Crimes Insight for Insurance
created: "2018-08-30"
modified: "2018-08-30"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/apis.md
specificationVersion: "0.14"
apis:
- name: Financial Crimes Insight for Insurance public REST APIs - Request a managed
    analysis to run
  x-api-slug: ibmfciplatformdata-accessanalysis-request-post
  description: This service can be used to initiate a managed analysis
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformdata-accessanalysis-request-post-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Submit assessments
    from monitored analytics
  x-api-slug: ibmfciplatformexternal-alertanalysis-result-post
  description: This method is used to submit analysis results from monitored analysis
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformexternal-alertanalysis-result-post-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Obtain security
    token for REST execution
  x-api-slug: ibmfciplatformtoken-servicetoken-get
  description: In addition to a username and password required to execute a REST service,
    the platform supports enhanced cross site scripting detection and requires a service
    token for REST API execution.  REST services will need to supply the token as
    both cookie and header in a REST request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformtoken-servicetoken-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformtoken-servicetoken-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Insert account data
    into the database
  x-api-slug: ibmfciplatformfactaccount-put
  description: This method is used to insert account data into the database.  The
    XML schema is defined in the ACCOUNT.XSD file.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactaccount-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactaccount-put-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Retrieve account
    data from the database, for the id
  x-api-slug: ibmfciplatformfactaccountid-get
  description: This method is used to retrieve account data from the database
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactaccountid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactaccountid-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Return the existing
    assessments for the object specified
  x-api-slug: ibmfciplatformfacttyperemotesystemremotekeyassessments-get
  description: This service is used to return the existing assessments for the object
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfacttyperemotesystemremotekeyassessments-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Retrieve set of
    identities considered to be the same entity
  x-api-slug: ibmfciplatformfactentityremote-system-idexternal-remote-reference-get
  description: This method is used to retrieve the set of individuals (or organizations)
    that are considered the same as the provided party reference
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactentityremote-system-idexternal-remote-reference-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Determine if one
    object is a match to the other.
  x-api-slug: ibmfciplatformfactmatch-get
  description: Using the provided objects, determine if one is a 'match' of the other
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactmatch-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Get a list of resolved
    objects from resolved entities for a given object.
  x-api-slug: ibmfciplatformfactentitymatch-get
  description: Get a list of resolved objects from resolved entities for a given object.
    Using the provided object ID, produce a list of all objects of the same business
    object type that have been determined to be 'matches'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactentitymatch-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Get the data for
    the resolved entity id.
  x-api-slug: ibmfciplatformfactentityid-get
  description: Using the provided party id, obtain the entity id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactentityid-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Search for objects
    that match the search terms specified.
  x-api-slug: ibmfciplatformfactentitysearch-post
  description: 'Search for objects that match the search terms specified.  The searchType
    refers to the type of object being searched for. Valid values include: Folio,Account,Event,Group,PhysicalObject,Party,Transaction,Any.
    Note that paging and ordering is not supported for type Any.  The parameter globalsearch
    represents a global search string with support for the * wildcard.  The propertysearch
    fields are a list of searches for matching on specified fields of an object.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactentitysearch-post-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - This method is used
    to retrieve the set of explicitly related parties and implicitly related entities
    for the supplied externally sourced reference party
  x-api-slug: ibmfciplatformfactentityrelatedpartiessystemidremotereference-get
  description: |-
    A data source must be configured in the appropriate server.xml to use ISII. Ensure that the following has been included:

    &lt;dataSource beginTranForResultSetScrollingAPIs="false" id="ISIIDB" isolationLevel="TRANSACTION_READ_COMMITTED" jndiName="jdbc/isii"&gt;

    &lt;jdbcDriver javax.sql.DataSource="com.ibm.db2.jcc.DB2XADataSource" libraryRef="DB2_LIB"/&gt;

    &lt;properties.db2.jcc databaseName="ISII" password="${isii_db_pass}" portNumber="${isii_db_port}" serverName="${isii_host}" user="${isii_db_user}"/&gt;

    &lt;connectionManager connectionTimeout="60s" maxIdleTime="3m" maxPoolSize="200" minPoolSize="0"/&gt;

    &lt;/dataSource&gt;

    Where password, portNumber, serverName, and user values are replaced with the appropriate properties or environment variables for your configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactentityrelatedpartiessystemidremotereference-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactentityrelatedpartiessystemidremotereference-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Insert event data
    into the database
  x-api-slug: ibmfciplatformfactevent-put
  description: This method is used to insert event data into the database.  The XML
    schema is defined in the EVENT.XSD file.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactevent-put-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Retrieve event data
    from the database, for the id
  x-api-slug: ibmfciplatformfacteventid-get
  description: This method is used to retrieve event data from the database
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfacteventid-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Insert group data
    into the database
  x-api-slug: ibmfciplatformfactgroup-put
  description: This method is used to insert group data into the database.  The XML
    schema is defined in the GROUP.XSD file.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactgroup-put-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Retrieve group data
    from the database, for the specific group id
  x-api-slug: ibmfciplatformfactgroupid-get
  description: This method is used to retrieve specific group data from the database
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactgroupid-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Insert party data
    into the database
  x-api-slug: ibmfciplatformfactparty-put
  description: This method is used to insert party data into the database.  The XML
    schema is defined in the PARTY.XSD file.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactparty-put-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Retrieve party data
    from the database, for the id
  x-api-slug: ibmfciplatformfactpartyid-get
  description: This method is used to retrieve party data from the database
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactpartyid-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Insert physical
    object data into the database
  x-api-slug: ibmfciplatformfactphysical-object-put
  description: This method is used to insert physical object data into the database.  The
    XML schema is defined in the PhysicalObject.XSD file.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactphysical-object-put-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Retrieve a specific
    physical object data from the database, based on its internal id
  x-api-slug: ibmfciplatformfactphysical-objectid-get
  description: This method is used to retrieve specific physical object data from
    the database, based on its internal id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactphysical-objectid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactphysical-objectid-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Screen a specific
    attribute against a dynamic list
  x-api-slug: ibmfciplatformfactscreen-get
  description: This method is used to screen data against a specific list of values,
    resulting in a JSON object containing a list of matching objects
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactscreen-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactscreen-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Insert transaction
    data into the database
  x-api-slug: ibmfciplatformfacttransaction-put
  description: This method is used to insert transaction data into the database.  The
    XML schema is defined in the TRANSACTION.XSD file.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfacttransaction-put-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Retrieve transaction
    data from the database, by its internal id
  x-api-slug: ibmfciplatformfacttransactionid-get
  description: This method is used to retrieve transaction data from the database
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfacttransactionid-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Retrieve a list
    of the registered watchlists
  x-api-slug: ibmfciplatformfactwatchlist-get
  description: This method is used to retrieve the list of registered watchlists from
    the database
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlist-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Persist the provided
    watchlist into the local database
  x-api-slug: ibmfciplatformfactwatchlist-post
  description: 'This method is used to persist the contents of a watchlist into the
    database.  Note: This method uses some data import functionality to create business
    object entries, then calls putWatchlist to create/update a watchlist for the provided
    identifier, and finally calls putWatchlistItem for every object created. This
    one also has the caveat of needing a disposition defined, but in this case all
    you need to pass in is the stereotype value.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlist-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlist-post-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Retrieve the contents
    of a watchlist, based on its id
  x-api-slug: ibmfciplatformfactwatchlistid-get
  description: This method is used to retrieve the contents of a watchlist from the
    database
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlistid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfactwatchlistid-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Retrieve details
    of a folio, by its internal id
  x-api-slug: ibmfciplatformfolio-managementfolioid-get
  description: This method is used to retrieve the folio contents from the database
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformfolio-managementfolioid-get-openapi.md
- name: Financial Crimes Insight for Insurance public REST APIs - Retrieve business
    objects using the specified parameters
  x-api-slug: ibmfciplatformlogical-objectsearch-post
  description: "This method provides searches for business objects within the database.
    \ The results for searching on a time stamp field are affected by the way that
    DB2\xC2\xAE handles time stamps. The JSON string uses ISO format for time stamps,
    such as 2016-06-15T20:11:19.326-04:00. DB2 converts this value to 2016-06-15-20.11.19.326000.
    Because DB2 might add more precision by storing a time stamp as 2016-06-15-20.11.19.326nnnn,
    the search results might not return what is expected. Refer to your DB2 documentation
    for more information on time stamps."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/WFS-Counter-Fraud-Technical-Level-3.png
  humanURL: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
  baseURL: https://fcihost.ibm.com:9443//
  tags: Policing, Financial, Insurance, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/ibmfciplatformlogical-objectsearch-post-openapi.md
x-common:
- type: x-openapi
  url: https://www.ibm.com/support/knowledgecenter/SSC2HF_3.0.0/api/fcii-insurance-v3.0.0.yaml?origin=swagger-ui
- type: x-pricing
  url: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN#echargex
- type: x-website
  url: https://www-01.ibm.com/common/ssi/cgi-bin/ssialias?infotype=AN&subtype=CA&htmlfid=897/ENUS218-305&appname=USN
- type: x-api-gallery
  url: http://ibm.cloud.api.gallery.streamdata.io
- type: x-api-stack
  url: http://ibm.financial.crimes.insight.for.insurance.stack.network
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---