{
  "info": {
    "name": "IBM Financial Crimes Insight for Insurance API This method is used to retrieve the set of explicitly related parties and implicitly related entities for the supplied externally sourced reference party",
    "_postman_id": "ca92c8ff-1cc5-44dd-ba38-15e93a034c89",
    "description": "A data source must be configured in the appropriate server.xml to use ISII. Ensure that the following has been included:\n\n&lt;dataSource beginTranForResultSetScrollingAPIs=\"false\" id=\"ISIIDB\" isolationLevel=\"TRANSACTION_READ_COMMITTED\" jndiName=\"jdbc/isii\"&gt;\n\n&lt;jdbcDriver javax.sql.DataSource=\"com.ibm.db2.jcc.DB2XADataSource\" libraryRef=\"DB2_LIB\"/&gt;\n\n&lt;properties.db2.jcc databaseName=\"ISII\" password=\"${isii_db_pass}\" portNumber=\"${isii_db_port}\" serverName=\"${isii_host}\" user=\"${isii_db_user}\"/&gt;\n\n&lt;connectionManager connectionTimeout=\"60s\" maxIdleTime=\"3m\" maxPoolSize=\"200\" minPoolSize=\"0\"/&gt;\n\n&lt;/dataSource&gt;\n\nWhere password, portNumber, serverName, and user values are replaced with the appropriate properties or environment variables for your configuration.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "This",
      "item": [
        {
          "id": "283fe3e0-c740-483f-8919-905e7287405b",
          "name": "getRelatedObjects",
          "request": {
            "url": {
              "protocol": "http",
              "host": "fcihost.ibm.com",
              "path": [
                "ibm/fci/platform/fact/entity/relatedparties/:systemId/:remoteReference"
              ],
              "port": "9443",
              "query": [
                {
                  "key": "minRelatedScore",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "remoteReference",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "systemId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "A data source must be configured in the appropriate server.xml to use ISII. Ensure that the following has been included:\n\n&lt;dataSource beginTranForResultSetScrollingAPIs=\"false\" id=\"ISIIDB\" isolationLevel=\"TRANSACTION_READ_COMMITTED\" jndiName=\"jdbc/isii\"&gt;\n\n&lt;jdbcDriver javax.sql.DataSource=\"com.ibm.db2.jcc.DB2XADataSource\" libraryRef=\"DB2_LIB\"/&gt;\n\n&lt;properties.db2.jcc databaseName=\"ISII\" password=\"${isii_db_pass}\" portNumber=\"${isii_db_port}\" serverName=\"${isii_host}\" user=\"${isii_db_user}\"/&gt;\n\n&lt;connectionManager connectionTimeout=\"60s\" maxIdleTime=\"3m\" maxPoolSize=\"200\" minPoolSize=\"0\"/&gt;\n\n&lt;/dataSource&gt;\n\nWhere password, portNumber, serverName, and user values are replaced with the appropriate properties or environment variables for your configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07cbdb7d-a1cd-41ea-a1a7-5f4c5d916ecb"
            }
          ]
        }
      ]
    }
  ]
}