{
  "info": {
    "name": "Gitter API Update Message",
    "_postman_id": "0b938248-b563-41a4-9f74-e688bb10b091",
    "description": "Update a message.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "1e0fefa0-d6ad-4547-bd54-82093ee8ff8a",
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
              "id": "0325d101-d69f-4c5e-8197-64399853b8e1"
            }
          ]
        }
      ]
    },
    {
      "name": "Rooms",
      "item": [
        {
          "id": "45b911b6-3429-4bb0-8b25-e8dcb0047555",
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
              "id": "52882d47-1d61-4a17-a5de-6602f28753bb"
            }
          ]
        },
        {
          "id": "1e17d21e-44c7-4a7a-998e-c730adc3f7c1",
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
              "id": "038b0993-a3e4-488a-84c2-37dbd8879b01"
            }
          ]
        },
        {
          "id": "7d500b54-e132-4ef1-b4ca-01e1260acd05",
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
              "id": "d9780c9e-0e58-4207-a1b2-ac27845ca39a"
            }
          ]
        },
        {
          "id": "f750cfc3-6276-4a8d-94ed-ac93cfcbfdaa",
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
              "id": "feab4b88-1d9b-4e53-a55b-2fcbd81b2856"
            }
          ]
        },
        {
          "id": "17885e79-7972-406a-8d2c-a99d45d19fb4",
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
              "id": "035443fe-3c6e-4f03-9644-4fa6a9f2326d"
            }
          ]
        },
        {
          "id": "6c5e1165-7860-4f98-bd48-a43f02d6712c",
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
              "id": "42ae0feb-a2ee-4797-8e03-b71d6dd15ffd"
            }
          ]
        },
        {
          "id": "86a65ccc-a2b0-43e7-bc5e-1177e83c6b8d",
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
              "id": "8e75bae9-e798-4890-9970-7fa7281b06ed"
            }
          ]
        },
        {
          "id": "8371d82e-4201-4360-b98d-629baf38ef63",
          "name": "sendMessage",
          "request": {
            "url": "http://example.com/api/rooms/:roomId/chatMessages?text=text",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Send a message to a room."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39db3ccc-ffaf-499e-9d59-e80020da974a"
            }
          ]
        },
        {
          "id": "efb9f2be-10aa-4643-97cc-81be3f16e866",
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
              "id": "eddbdc75-d898-4a85-b61b-0c625b25d956"
            }
          ]
        },
        {
          "id": "da5bafb9-4de9-4510-86d3-47d8c357e2f1",
          "name": "updateMessage",
          "request": {
            "url": "http://example.com/api/rooms/:roomId/chatMessages/:chatMessageId?text=text",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a51a18e3-22f9-476d-84b5-36560eea7ded"
            }
          ]
        }
      ]
    }
  ]
}