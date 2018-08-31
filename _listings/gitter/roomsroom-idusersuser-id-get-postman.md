{
  "info": {
    "name": "Gitter API Remove Room",
    "_postman_id": "ffde495b-115e-4003-8183-6af6c87ef7fc",
    "description": "Remove a user from a room.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "80895532-164c-46f3-a566-4df3469bd3bf",
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
              "id": "ba0f0f32-2f2a-4c91-a7eb-7ff3b4cbf0ef"
            }
          ]
        }
      ]
    },
    {
      "name": "Rooms",
      "item": [
        {
          "id": "c509affc-98de-4370-b005-f14111e09605",
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
              "id": "f2975a9b-0587-4a1f-87cb-28f5b1944f8e"
            }
          ]
        },
        {
          "id": "f301b3b5-6cf5-4a8e-8b46-424e2e647565",
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
              "id": "8de1f286-f4e2-4abd-9ad4-9ef60fb0b803"
            }
          ]
        },
        {
          "id": "5b395423-d98e-4b8d-a4a2-0228dd9faa5e",
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
              "id": "c8adf94d-853b-43ab-bbdf-d958502ba95e"
            }
          ]
        }
      ]
    }
  ]
}