{
  "info": {
    "name": "Gitter API Send Message",
    "_postman_id": "6457630e-fbec-412a-a4be-63c97d005f39",
    "description": "Send a message to a room.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "d3d15d4d-ecd9-4644-a0b3-2471ab7ee18a",
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
              "id": "292b1084-f704-4d64-8c56-927adcfb8c5d"
            }
          ]
        }
      ]
    },
    {
      "name": "Rooms",
      "item": [
        {
          "id": "44b728b1-3dfb-41d8-8a2e-aee37df667d1",
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
              "id": "2b03ac08-90e8-4c45-927d-fbd4457b0bda"
            }
          ]
        },
        {
          "id": "32e16568-634d-4cd2-a9af-478fc59ad0a7",
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
              "id": "b08e3193-6a65-4e0e-ae1d-5ac60c2a874b"
            }
          ]
        },
        {
          "id": "c01c6803-e5dc-4623-9818-8a0e68bebd0e",
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
              "id": "f38b4eb4-9d3c-4057-8275-eeb962df95ee"
            }
          ]
        },
        {
          "id": "aecffc07-1565-4127-b2d1-33f35881053b",
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
              "id": "f278fa23-6ff5-48cd-9821-3b12fb8b0578"
            }
          ]
        },
        {
          "id": "39a68bf7-9da2-4a76-a48e-3c0b8ac4a092",
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
              "id": "290817ad-d364-414b-8344-7f0db2701fef"
            }
          ]
        },
        {
          "id": "9b3507d7-0573-44b9-aee8-010895a45bf2",
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
              "id": "b7785537-ffef-4eb5-99af-dbb2a4cfe05b"
            }
          ]
        },
        {
          "id": "ffde43cc-0fa3-4048-b562-d997e20bedc9",
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
              "id": "68bd0d12-2cec-48e7-9865-b70a2dbd21d2"
            }
          ]
        },
        {
          "id": "9139cd3e-e951-417d-993c-72e65c75ea63",
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
              "id": "a343255a-d886-4a6a-90a6-73026832eb6e"
            }
          ]
        },
        {
          "id": "4a7a6ee8-b814-485c-917e-338162eab9cc",
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
              "id": "5d8f3fbc-fb6c-4354-b577-908d0ef02f08"
            }
          ]
        }
      ]
    }
  ]
}