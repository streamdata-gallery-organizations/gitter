{
  "info": {
    "name": "Gitter API Get Room Message",
    "_postman_id": "393bc4f1-13e8-45a4-a932-1d3e1db34b85",
    "description": "There is also a way to retrieve a single message using its id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "80afb0dc-7de4-4773-a530-97cf5111a09f",
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
              "id": "c2c9764b-6492-4204-9d52-4c054fd8d8d0"
            }
          ]
        }
      ]
    },
    {
      "name": "Rooms",
      "item": [
        {
          "id": "1879f9e9-9a2b-49fe-8930-accbfb5cc706",
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
              "id": "d6f58917-009e-4699-9c5f-c887eec42c5f"
            }
          ]
        },
        {
          "id": "692fbc38-3ab5-4171-96de-f299e254a020",
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
              "id": "0e6bd4b4-4b09-4501-8387-22d4c87f22aa"
            }
          ]
        },
        {
          "id": "df4d3358-1f4d-4568-8748-35f9b1f93700",
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
              "id": "ffb41762-d581-4d81-aa8b-f8ff012fd2b1"
            }
          ]
        },
        {
          "id": "605b99ce-ddaa-4522-8999-f1b03bdaa776",
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
              "id": "0b382ed9-235a-4f95-bb9b-f4ccb6f7a7f4"
            }
          ]
        },
        {
          "id": "cb0ef6e6-9f0a-40b4-a910-854811315bf2",
          "name": "deleteRoom",
          "request": {
            "url": "http://example.com/api/rooms/:roomId",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a room."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6bf63d4-3956-4ee9-ae9b-ea0adbbc36d0"
            }
          ]
        },
        {
          "id": "d2f4e9ae-ca1d-48c4-845e-8a8487ecd32b",
          "name": "getRoomUsers",
          "request": {
            "url": "http://example.com/api/rooms/:roomId/users?limit=limit&q=q&skip=skip",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of Users currently in the room."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b56757cd-e1b3-4530-91ce-fa436b55132a"
            }
          ]
        },
        {
          "id": "344f87bc-7a62-4574-92c3-33dad5eab41d",
          "name": "listRoomMessages",
          "request": {
            "url": "http://example.com/api/rooms/:roomId/chatMessages?afterId=afterId&aroundId=aroundId&beforeId=beforeId&limit=limit&q=q&skip=skip",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of messages in a room."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d08933ba-5594-4821-aa69-fbbd820056f8"
            }
          ]
        },
        {
          "id": "95f0e0eb-b50b-4ac1-8fbd-cdf85ec15793",
          "name": "getRoomMessage",
          "request": {
            "url": "http://example.com/api/rooms/:roomId/chatMessages/:messageId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "There is also a way to retrieve a single message using its id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "589197b0-f63d-43c8-9122-0712387a2e28"
            }
          ]
        }
      ]
    }
  ]
}