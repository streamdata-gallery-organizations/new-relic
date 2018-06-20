{
  "info": {
    "name": "New Relic Get Components Component  Metrics. Format",
    "_postman_id": "bf7bff7c-5beb-4154-b8ef-699cb4017843",
    "description": "Return a list of known metrics and their value names for the given resource.\n\nSee our documentation for a discussion\non  output pagination\nand for examples of requesting and using metric values.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Components.",
      "item": [
        {
          "id": "3f4999eb-7494-45ca-b1a0-66398f9dfb82",
          "name": "getComponents.Format",
          "request": {
            "url": "http://example.com/v2/components.json?filter[ids]=%7B%7D&filter[name]=filter%5Bname%5D&filter[plugin_id]=45&page=45",
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
              "id": "ca25b06f-eabc-48b3-8d6a-b7b30441a0ec"
            }
          ]
        }
      ]
    },
    {
      "name": "Components",
      "item": [
        {
          "id": "275573c1-a93b-44c5-98e9-0fd9339ff22e",
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
                  "value": "45",
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
              "id": "e9e9249e-04df-458b-a59a-6e3a563469eb"
            }
          ]
        },
        {
          "id": "f4ac7ec0-0590-4e62-84fc-98616d5d8d98",
          "name": "getComponentsComponentMetrics.Format",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "v2",
                "components/:component_id/metrics.json"
              ],
              "query": [
                {
                  "key": "cursor",
                  "value": "cursor",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "name",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "45",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "component_id",
                  "value": "45",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return a list of known metrics and their value names for the given resource.\n\nSee our documentation for a discussion\non  output pagination\nand for examples of requesting and using metric values."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "06dc4470-736a-4311-b2b9-fa363a4689d4"
            }
          ]
        }
      ]
    }
  ]
}