{
  "info": {
    "name": "IBM Financial Crimes Insight for Insurance API Retrieve the contents of a watchlist, based on its id",
    "_postman_id": "9ab2866f-9c23-4ca1-84a2-0d2a6b1248b2",
    "description": "This method is used to retrieve the contents of a watchlist from the database",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Retrieve",
      "item": [
        {
          "id": "ca46629d-e8ad-4de1-9202-6a7088edac40",
          "name": "getPhysicalObject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "fcihost.ibm.com",
              "path": [
                "ibm/fci/platform/fact/physical_object/:id"
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
            "description": "This method is used to retrieve specific physical object data from the database, based on its internal id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "966fbeb7-008a-4f4f-9967-8a1cb80ed029"
            }
          ]
        },
        {
          "id": "a2ba6a2d-0bc9-4786-b3a1-e896c73e51fd",
          "name": "getWatchlistById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "fcihost.ibm.com",
              "path": [
                "ibm/fci/platform/fact/watchlist/:id"
              ],
              "port": "9443",
              "query": [
                {
                  "key": "summary",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
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
            "description": "This method is used to retrieve the contents of a watchlist from the database"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb54e190-dca5-4fa4-aab8-0efc4e3dc6e8"
            }
          ]
        }
      ]
    }
  ]
}