{
  "info": {
    "name": "New Relic Get Components Component  Metrics Data. Format",
    "_postman_id": "10311383-83a7-44ae-8c0e-4542ecf2804b",
    "description": "This API endpoint returns a list of values for each of the requested metrics. The list of available metrics\ncan be returned using the Metric Name API endpoint.\n\nMetric data can be filtered by a number of parameters, including multiple names and values, and by time range.\nMetric names and values will be matched intelligently in the background.\n\nYou can also retrieve a summarized data point across the entire time range selected by using the summarize\nparameter.\n\nSee our documentation for a discussion on \noutput pagination,  time range \nrelated considerations, and for examples of requesting and using metric values.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Components.",
      "item": [
        {
          "id": "41ba9891-1b73-49de-a469-178d18dab703",
          "name": "getComponents.Format",
          "request": {
            "url": "http://example.com/v2/components.json?filter[ids]=%7B%7D&filter[name]=filter%5Bname%5D&filter[plugin_id]=112&page=112",
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
              "id": "29989b24-f852-4bfa-afbf-c39b45dced76"
            }
          ]
        }
      ]
    },
    {
      "name": "Components",
      "item": [
        {
          "id": "bcf610e9-73da-43fb-baa8-504232de861f",
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
                  "value": "112",
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
              "id": "3f1d2b36-ace4-4f06-b648-0b8ca038e3b2"
            }
          ]
        },
        {
          "id": "6590ac68-0816-4f36-96b5-d30fddea022c",
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
                  "value": "112",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "component_id",
                  "value": "112",
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
              "id": "e409f351-aead-4982-a5f9-4a3c8e7d3b03"
            }
          ]
        },
        {
          "id": "fa66277c-1fcb-45fb-8c55-e6372d2aedf4",
          "name": "getComponentsComponentMetricsData.Format",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "v2",
                "components/:component_id/metrics/data.json"
              ],
              "query": [
                {
                  "key": "from",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "names",
                  "value": "%5B%22names%22%5D",
                  "disabled": false
                },
                {
                  "key": "period",
                  "value": "112",
                  "disabled": false
                },
                {
                  "key": "raw",
                  "value": "false",
                  "disabled": false
                },
                {
                  "key": "summarize",
                  "value": "false",
                  "disabled": false
                },
                {
                  "key": "to",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "values",
                  "value": "%5B%22values%22%5D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "component_id",
                  "value": "112",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API endpoint returns a list of values for each of the requested metrics. The list of available metrics\ncan be returned using the Metric Name API endpoint.\n\nMetric data can be filtered by a number of parameters, including multiple names and values, and by time range.\nMetric names and values will be matched intelligently in the background.\n\nYou can also retrieve a summarized data point across the entire time range selected by using the summarize\nparameter.\n\nSee our documentation for a discussion on \noutput pagination,  time range \nrelated considerations, and for examples of requesting and using metric values."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d443c4e0-0dd8-4c8e-99a7-4b9976f2b7b7"
            }
          ]
        }
      ]
    }
  ]
}