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
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ibm-financial-crimes-insight-for-insurance/master/_listings/ibm-financial-crimes-insight-for-insurance/apis.md
specificationVersion: "0.14"
apis:
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