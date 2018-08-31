{
  "info": {
    "name": "New Relic Put Alerts Policy Channels. Format",
    "_postman_id": "fd137285-45df-4971-b88f-9e29970f3bc3",
    "description": "This API endpoint updates policy/channel associations.\n\nNote: Admin User???s API Key is required.\n\nSee our documentation for a discussion on updating notification channels with policies.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Alerts",
      "item": [
        {
          "id": "034a938f-168b-4a1e-9493-977c38aa9284",
          "name": "putAlertsPolicyChannels.Format",
          "request": {
            "url": "http://example.com/v2/alerts_policy_channels.json?channel_ids=%7B%7D&policy_id=69",
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
              "id": "f7c68468-47af-426b-a0f4-e6c9bdd44220"
            }
          ]
        }
      ]
    }
  ]
}