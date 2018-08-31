{
  "info": {
    "name": "New Relic Get Alerts Channels. Format",
    "_postman_id": "4bd61e78-09ea-4e6a-b8c0-41591fe17f10",
    "description": "This API endpoint works with new Alerts on alerts.newrelic.com.\n\nIt returns a list of the channels associated with your New Relic account.\n\nSee our documentation for a discussion on listing notification channels.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Alerts",
      "item": [
        {
          "id": "22e083f7-1114-4195-bcc3-85b0b8763cee",
          "name": "putAlertsPolicyChannels.Format",
          "request": {
            "url": "http://example.com/v2/alerts_policy_channels.json?channel_ids=%7B%7D&policy_id=231",
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
              "id": "09d915aa-0051-432a-978d-489a0da814cb"
            }
          ]
        },
        {
          "id": "e17fe9ca-1b56-4afb-9582-275b92bb3a3d",
          "name": "deleteAlertsPolicyChannels.Format",
          "request": {
            "url": "http://example.com/v2/alerts_policy_channels.json?channel_id=231&policy_id=231",
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
              "id": "5448b54b-0e1f-424b-950a-5570de9aa63a"
            }
          ]
        },
        {
          "id": "9f79d990-9e74-43f9-9884-a8a36cb4c924",
          "name": "getAlertsChannels.Format",
          "request": {
            "url": "http://example.com/v2/alerts_channels.json?page=231",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API endpoint works with new Alerts on alerts.newrelic.com.\n\nIt returns a list of the channels associated with your New Relic account.\n\nSee our documentation for a discussion on listing notification channels."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d55a6d40-75f3-4865-8b29-7a3483af4250"
            }
          ]
        }
      ]
    }
  ]
}