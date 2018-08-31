{
  "info": {
    "name": "New Relic Delete Alerts Policy Channels. Format",
    "_postman_id": "0420784e-fb4f-4007-a517-cb1e6dcaf1be",
    "description": "This API endpoint deletes Alerts policy/channel associations.\n\nNote: Admin User???s API Key is required.\n\nSee our documentation for a discussion on deleting notification channels with policies.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Alerts",
      "item": [
        {
          "id": "0c54ad97-afb2-43f4-ab1b-07743b961d39",
          "name": "putAlertsPolicyChannels.Format",
          "request": {
            "url": "http://example.com/v2/alerts_policy_channels.json?channel_ids=%7B%7D&policy_id=114",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "This API endpoint updates policy/channel associations.\n\nNote: Admin User???s API Key is required.\n\nSee our documentation for a discussion on updating notification channels with policies."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a92a1175-e0d5-4759-badc-53f1569ab7fa"
            }
          ]
        },
        {
          "id": "bcf5dff2-891f-4a5f-a528-4b2bee03a815",
          "name": "deleteAlertsPolicyChannels.Format",
          "request": {
            "url": "http://example.com/v2/alerts_policy_channels.json?channel_id=114&policy_id=114",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "This API endpoint deletes Alerts policy/channel associations.\n\nNote: Admin User???s API Key is required.\n\nSee our documentation for a discussion on deleting notification channels with policies."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7587e22a-a8b9-4701-a73b-a3cb5c38b8c4"
            }
          ]
        }
      ]
    }
  ]
}