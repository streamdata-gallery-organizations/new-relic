{
  "info": {
    "name": "New Relic Get Components  . Format",
    "_postman_id": "92229b66-6315-4c03-92ea-f74d75ff1c12",
    "description": "This API endpoint returns a single component, identified by its ID.\n\nSee our documentation for a discussion on listing components by ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Components.",
      "item": [
        {
          "id": "c5f31c3a-c630-4ec2-866f-e8c2e16fcb9d",
          "name": "getComponents.Format",
          "request": {
            "url": "http://example.com/v2/components.json?filter[ids]=%7B%7D&filter[name]=filter%5Bname%5D&filter[plugin_id]=232&page=232",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API endpoint returns a list of the plugin components associated with your New Relic account.\n\nPlugins can be filtered by their name, the list of component IDs or a plugin ID.\n\nSee our documentation for a discussion on  listing components\nand  output pagination."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4dc7666f-738e-4951-b4de-e1c787e0eb05"
            }
          ]
        }
      ]
    },
    {
      "name": "Components",
      "item": [
        {
          "id": "c06fe133-fd0a-4345-94f0-afb6a9871f20",
          "name": "getComponents.Format",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "v2",
                "components/:id.json"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "232",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API endpoint returns a single component, identified by its ID.\n\nSee our documentation for a discussion on listing components by ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2cab2238-e705-42eb-8d00-3fbc9b32f961"
            }
          ]
        }
      ]
    }
  ]
}