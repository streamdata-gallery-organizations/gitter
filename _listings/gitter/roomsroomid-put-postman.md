{
  "info": {
    "name": "Gitter API Update room",
    "_postman_id": "dc56478d-d56d-40f5-bca8-74e7c82604fa",
    "description": "Updates a room.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "1b00078c-2d23-45cf-b97f-53f9f2601640",
          "name": "getGroupRooms",
          "request": {
            "url": "http://example.com/api/groups/:groupId/rooms",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List rooms under group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b00b726c-da12-4ed6-afd8-4c722fd30d1b"
            }
          ]
        }
      ]
    },
    {
      "name": "Rooms",
      "item": [
        {
          "id": "50634d30-7992-4771-9fc7-0c2a7e39f1fb",
          "name": "listRooms",
          "request": {
            "url": "http://example.com/api/rooms",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List rooms the current user is in."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72d40617-bb3f-4cd4-bb84-ade93f4be8d4"
            }
          ]
        },
        {
          "id": "af366e2d-821c-4461-9b80-d17676f35e5e",
          "name": "joinRoom",
          "request": {
            "url": "http://example.com/api/user/:userId/rooms",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "To join a room you'll need to provide a URI for it. Said URI can represent a GitHub Org, a GitHub Repo or a Gitter Channel."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "721b84b2-71a9-4c76-8839-b9db2329894a"
            }
          ]
        },
        {
          "id": "484cf08c-c799-47d6-a680-b3ac9a69cbbd",
          "name": "removeRoom",
          "request": {
            "url": "http://example.com/api/rooms/:room_id/users/:user_id",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Remove a user from a room."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bcc529df-7753-4b13-b2d9-9f74e8930508"
            }
          ]
        },
        {
          "id": "4105eb6a-9732-41f3-849f-44dae4d918e3",
          "name": "updateRoom",
          "request": {
            "url": "http://example.com/api/rooms/:roomId?noindex=noindex&tags=tags&topic=topic",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a room."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "19b3332d-d388-4b36-8440-a0f17c899e50"
            }
          ]
        }
      ]
    }
  ]
}