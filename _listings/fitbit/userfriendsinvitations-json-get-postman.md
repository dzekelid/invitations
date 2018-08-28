{
  "info": {
    "name": "Fitbit Get User Friends Invitations.json",
    "_postman_id": "525e1f55-a8bc-4691-8ea0-634c1cf7244a",
    "description": "Retrieve the list of invites to become freinds for a user in the format requested.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "c0be19d7-c069-4085-a073-f9f594530e07",
          "name": "getUserFriendsInvitations.json",
          "request": {
            "url": "http://api.fitbit.com/1/user/-/friends/invitations.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the list of invites to become freinds for a user in the format requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da5334ad-0965-4021-90e7-78ab523c4cfe"
            }
          ]
        }
      ]
    }
  ]
}