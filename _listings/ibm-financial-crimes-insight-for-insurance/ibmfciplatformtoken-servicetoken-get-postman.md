{
  "info": {
    "name": "IBM Financial Crimes Insight for Insurance API Obtain security token for REST execution",
    "_postman_id": "f7c697bc-ded1-4d42-ae69-35d631765433",
    "description": "In addition to a username and password required to execute a REST service, the platform supports enhanced cross site scripting detection and requires a service token for REST API execution.  REST services will need to supply the token as both cookie and header in a REST request.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Obtain",
      "item": [
        {
          "id": "a2f78726-0421-421f-9f93-54562da79231",
          "name": "getServiceToken",
          "request": {
            "url": "http://fcihost.ibm.com:9443/ibm/fci/platform/token_service/token",
            "method": "GET",
            "header": [
              {
                "key": "IBM-FCI-Role",
                "value": "{}",
                "description": "Userid / password for user with appropriate role",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "In addition to a username and password required to execute a REST service, the platform supports enhanced cross site scripting detection and requires a service token for REST API execution.  REST services will need to supply the token as both cookie and header in a REST request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1645efac-814f-4864-9742-abbe86d9de1d"
            }
          ]
        }
      ]
    }
  ]
}