{
  "info": {
    "name": "Azure CDN API List Resource Usage",
    "_postman_id": "293fa321-b5e6-45a8-bcf3-fd70b8378d53",
    "description": "Check the quota and actual usage of the CDN profiles under the given subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "cdn",
      "item": [
        {
          "id": "bb5be0d1-7a47-4e9d-b45c-25d677abcaa8",
          "name": "ListResourceUsage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Cdn/checkResourceUsage"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Check the quota and actual usage of the CDN profiles under the given subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2c5440f-212f-4c71-a96d-454830b2c9a0"
            }
          ]
        }
      ]
    }
  ]
}