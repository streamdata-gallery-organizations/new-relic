{
  "info": {
    "name": "New Relic Get Components. Format",
    "_postman_id": "b3074179-65e2-405a-a0fd-015998c714bc",
    "description": "This API endpoint returns a list of the plugin components associated with your New Relic account.\n\nPlugins can be filtered by their name, the list of component IDs or a plugin ID.\n\nSee our documentation for a discussion on  listing components\nand  output pagination.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Components.",
      "item": [
        {
          "id": "ab979b32-b3b9-4a9a-acbc-5543e6e6296d",
          "name": "getComponents.Format",
          "request": {
            "url": "http://example.com/v2/components.json?filter[ids]=%7B%7D&filter[name]=filter%5Bname%5D&filter[plugin_id]=109&page=109",
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
              "id": "792f8847-7dbc-4752-9efe-d20cfb9f3d3a"
            }
          ]
        }
      ]
    }
  ]
}