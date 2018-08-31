{
  "info": {
    "name": "New Relic Get Key Transactions. Format",
    "_postman_id": "9372faa8-4a1e-4f32-844c-8c3277e38afc",
    "description": "This API endpoint returns a paginated \nlist of the key transactions associated with your New Relic account.  The time range for summary data is the last 10 minutes.\n\nKey transactions can be filtered by their name or list of IDs.\n\nSee our documentation for a discussion of \nsummary data output.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Key",
      "item": [
        {
          "id": "c0833029-28d3-4eac-8731-61a0e96fc600",
          "name": "getKeyTransactions.Format",
          "request": {
            "url": "http://example.com/v2/key_transactions.json?filter[ids]=%7B%7D&filter[name]=filter%5Bname%5D&page=87",
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
              "id": "f07f15ac-da0f-425f-aa90-03d3ad6f51c0"
            }
          ]
        }
      ]
    }
  ]
}