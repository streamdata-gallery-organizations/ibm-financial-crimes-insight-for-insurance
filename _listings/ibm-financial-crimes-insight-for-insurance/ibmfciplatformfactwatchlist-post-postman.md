{
  "info": {
    "name": "IBM Financial Crimes Insight for Insurance API Persist the provided watchlist into the local database",
    "_postman_id": "41e56892-a54e-47b4-9db0-699a822c1d76",
    "description": "This method is used to persist the contents of a watchlist into the database.  Note: This method uses some data import functionality to create business object entries, then calls putWatchlist to create/update a watchlist for the provided identifier, and finally calls putWatchlistItem for every object created. This one also has the caveat of needing a disposition defined, but in this case all you need to pass in is the stereotype value.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Persist",
      "item": [
        {
          "id": "48575222-3e12-4ecc-95a4-8d7d678172c8",
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
              "id": "26a78792-c793-4322-b61b-271a872e9c14"
            }
          ]
        }
      ]
    }
  ]
}