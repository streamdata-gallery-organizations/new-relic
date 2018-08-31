{
  "info": {
    "name": "New Relic Get Applications Application  Deployments. Format",
    "_postman_id": "9fd21b64-ca6c-47fb-b41b-16ba74dde3d6",
    "description": "This API endpoint returns a paginated list of the deployments associated with a given application.\n\nSee our documentation for a discussion on output pagination.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Applications",
      "item": [
        {
          "id": "644bae0c-a952-45a7-aab7-c73bc5afe7c3",
          "name": "getApplicationsApplicationDeployments.Format",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "v2",
                "applications/:application_id/deployments.json"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "55",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "application_id",
                  "value": "55",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API endpoint returns a paginated list of the deployments associated with a given application.\n\nSee our documentation for a discussion on output pagination."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae7ddb8c-dbb3-4d6f-857c-502e83357b1d"
            }
          ]
        }
      ]
    }
  ]
}