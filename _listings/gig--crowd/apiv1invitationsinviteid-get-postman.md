{
  "info": {
    "name": "GIGANDCROWD Get Invitations Inviteid",
    "_postman_id": "19b41755-146d-4fa4-9f27-88278cb66eec",
    "description": "Get invitations inviteid.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Invitations",
      "item": [
        {
          "id": "6be125b7-2226-4eb6-af2b-6f07d00f639d",
          "name": "getApiV1InvitationsInvite",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/invitations/:inviteId"
              ],
              "variable": [
                {
                  "id": "inviteId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get invitations inviteid."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e339d92-11a1-4e0e-8f32-e61c70915787"
            }
          ]
        }
      ]
    }
  ]
}