{
  "info": {
    "name": "Gitter API Get User Rooms",
    "_postman_id": "ce3ebd5d-abdd-4370-87ae-516cd7f38950",
    "description": "List of Rooms the user is part of.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "342f629b-0e64-43dc-904b-e5f3a918a6c8",
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
              "id": "90e2dda8-d156-42bd-a79e-c8c12a9f0144"
            }
          ]
        }
      ]
    },
    {
      "name": "Rooms",
      "item": [
        {
          "id": "7751fe31-6a86-438e-b970-4e68f740dd3b",
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
              "id": "0642b321-e1ac-4c04-b6cb-041daf37473e"
            }
          ]
        },
        {
          "id": "3212f58e-9d20-4630-b41c-f19bc880df51",
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
              "id": "8f37c6ce-6b94-4666-a991-d9e876324435"
            }
          ]
        },
        {
          "id": "e43b742d-4d16-41ed-bdc5-cc61ff1cc698",
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
              "id": "04e12f93-4e23-4931-80fb-6c2375189466"
            }
          ]
        },
        {
          "id": "2daaa492-9370-4d8b-8739-930e14b1efc1",
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
              "id": "1bd4a3cd-4b20-4fdc-88b2-71445b2c8b76"
            }
          ]
        },
        {
          "id": "96387463-1cc3-4c87-98d5-a99521e58c4b",
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
              "id": "d1d4a062-6f77-46e8-ba68-3fb65dabf354"
            }
          ]
        },
        {
          "id": "f7f0cf22-76e0-43ab-aaa6-2467f73c1a8f",
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
              "id": "2b302583-e22f-4e55-b101-974a4217d59a"
            }
          ]
        },
        {
          "id": "0ae85006-167e-4ce8-a67e-1da6e92eeb53",
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
              "id": "625d9576-3fda-4c0d-bad9-8e5ef80fbb52"
            }
          ]
        },
        {
          "id": "e639af13-548f-4ee3-ae87-9cc8a36293cc",
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
              "id": "865d9d20-7f0d-4c12-a45c-6f9a033b2e01"
            }
          ]
        },
        {
          "id": "f0dcecf1-0b15-4f49-a5dc-68bd34edfefd",
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
              "id": "7a3c52b3-d9b7-4e59-bacd-bb48a0780679"
            }
          ]
        },
        {
          "id": "9e1ff9ee-f576-41af-beb1-5c41987cd214",
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
              "id": "ed8f92cc-8056-4d29-ae65-f8e3f6aa01e5"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "287aa220-9fc3-4a06-a52a-b7c849917373",
          "name": "getUserRooms",
          "request": {
            "url": "http://example.com/api/user/:userId/rooms",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of Rooms the user is part of."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "344af6f0-4e73-4203-bbe2-7283f898b6ed"
            }
          ]
        }
      ]
    }
  ]
}