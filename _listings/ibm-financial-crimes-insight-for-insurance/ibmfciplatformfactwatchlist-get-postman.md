{
  "info": {
    "name": "IBM Financial Crimes Insight for Insurance API Retrieve a list of the registered watchlists",
    "_postman_id": "1483c697-26f5-4e0d-b946-d0f19f388f72",
    "description": "This method is used to retrieve the list of registered watchlists from the database",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Retrieve",
      "item": [
        {
          "id": "925cc729-79dc-4ea4-b7a4-321beb4a697e",
          "name": "getWatchlists",
          "request": {
            "url": "http://fcihost.ibm.com:9443/ibm/fci/platform/fact/watchlist",
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
            "description": "This method is used to retrieve the list of registered watchlists from the database"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fdd3ffde-035c-4804-94a1-e949c400163d"
            }
          ]
        },
        {
          "id": "c2bff0b6-3e0e-4e5d-9635-253fae2b20b0",
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
              "id": "690b9f84-52e5-4159-a18d-5169542576bf"
            }
          ]
        }
      ]
    },
    {
      "name": "Persist",
      "item": [
        {
          "id": "7917aa06-daa9-45eb-95eb-985a6fa8191a",
          "name": "uploadWatchlist",
          "request": {
            "url": "http://fcihost.ibm.com:9443/ibm/fci/platform/fact/watchlist?disposition=%7B%7D&identifier=%7B%7D&overwrite=%7B%7D",
            "method": "POST",
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
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "data",
                  "value": "{}",
                  "disabled": false,
                  "description": "CSV file containing an external watchlist"
                },
                {
                  "key": "dataName",
                  "value": "{}",
                  "disabled": false,
                  "description": "CSV file name"
                },
                {
                  "key": "properties",
                  "value": "{}",
                  "disabled": false,
                  "description": "A"
                },
                {
                  "key": "propertiesName",
                  "value": "{}",
                  "disabled": false,
                  "description": "Properties file name"
                }
              ]
            },
            "description": "This method is used to persist the contents of a watchlist into the database.  Note: This method uses some data import functionality to create business object entries, then calls putWatchlist to create/update a watchlist for the provided identifier, and finally calls putWatchlistItem for every object created. This one also has the caveat of needing a disposition defined, but in this case all you need to pass in is the stereotype value."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4840dff2-0d79-4f8d-884e-a87faf57f8a5"
            }
          ]
        }
      ]
    }
  ]
}