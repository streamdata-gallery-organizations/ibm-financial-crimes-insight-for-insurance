{
  "info": {
    "name": "IBM Financial Crimes Insight for Insurance API Insert account data into the database",
    "_postman_id": "2fc19859-c3cd-4024-89d1-a3e9bb5032cb",
    "description": "This method is used to insert account data into the database.  The XML schema is defined in the ACCOUNT.XSD file.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Insert",
      "item": [
        {
          "id": "c22286a2-c5a7-454e-86b4-90559c84ef40",
          "name": "putAccount",
          "request": {
            "url": "http://fcihost.ibm.com:9443/ibm/fci/platform/fact/account",
            "method": "PUT",
            "header": [
              {
                "key": "IBM-FCI-Role",
                "value": "{}",
                "description": "Userid / password for user with appropriate role",
                "disabled": false
              },
              {
                "key": "IBM-FCI-Token",
                "value": "{}",
                "description": "Security token obtained for execution",
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
            "description": "This method is used to insert account data into the database.  The XML schema is defined in the ACCOUNT.XSD file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cfcc79d8-632f-4dec-9c1b-cd4f4a88f329"
            }
          ]
        }
      ]
    },
    {
      "name": "Retrieve",
      "item": [
        {
          "id": "9b6174a6-e41c-40b2-9b4c-089b279d6d35",
          "name": "getAccount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "fcihost.ibm.com",
              "path": [
                "ibm/fci/platform/fact/account/:id"
              ],
              "port": "9443",
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "IBM-FCI-Role",
                "value": "{}",
                "description": "Userid / password for user with appropriate role",
                "disabled": false
              },
              {
                "key": "IBM-FCI-Token",
                "value": "{}",
                "description": "Security token obtained for execution",
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
            "description": "This method is used to retrieve account data from the database"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "967688d3-9741-4d99-a957-6c90bebb5f52"
            }
          ]
        }
      ]
    }
  ]
}