{
  "info": {
    "name": "New Relic Get Key Transactions  . Format",
    "_postman_id": "6f3e7427-0fe9-43e5-855b-5271e0cb75eb",
    "description": "This endpoint returns a single key transaction, identified by ID. The time range for summary data is the last 10 minutes.\n\nSee our documentation for a discussion of \nsummary data output.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Key",
      "item": [
        {
          "id": "d210280b-a62d-456d-88d4-322eaf5fb265",
          "name": "getKeyTransactions.Format",
          "request": {
            "url": "http://example.com/v2/key_transactions.json?filter[ids]=%7B%7D&filter[name]=filter%5Bname%5D&page=205",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API endpoint returns a paginated \nlist of the key transactions associated with your New Relic account.  The time range for summary data is the last 10 minutes.\n\nKey transactions can be filtered by their name or list of IDs.\n\nSee our documentation for a discussion of \nsummary data output."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8b9600e-f8af-4d1f-bfbe-fd31fa4435c0"
            }
          ]
        },
        {
          "id": "92587da3-6079-4f6b-97a8-13ace299fdb3",
          "name": "getKeyTransactions.Format",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "v2",
                "key_transactions/:id.json"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "205",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint returns a single key transaction, identified by ID. The time range for summary data is the last 10 minutes.\n\nSee our documentation for a discussion of \nsummary data output."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5940a71b-0b75-4d8c-bcc3-afea96165e65"
            }
          ]
        }
      ]
    }
  ]
}