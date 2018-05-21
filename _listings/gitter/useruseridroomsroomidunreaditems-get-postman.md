{
  "info": {
    "name": "Gitter API Get User Unread Items",
    "_postman_id": "7fc38f18-7c31-4565-aff7-184819bde270",
    "description": "You can retrieve unread items and mentions using the following endpoint.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "302a6b8c-4b76-43ed-bd9b-15e8a69c58b4",
          "name": "listGroups",
          "request": {
            "url": "http://example.com/api/groups",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List groups the current user is in."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c42a070a-a597-4a9b-98a8-09d99841b8a2"
            }
          ]
        },
        {
          "id": "0cbdf361-49ac-435d-ba0f-c9c608634426",
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
              "id": "60a297c0-44de-4d2c-88e1-dfc36c2cd701"
            }
          ]
        }
      ]
    },
    {
      "name": "Rooms",
      "item": [
        {
          "id": "76b47c3d-41da-44f0-87c9-3ba8a97c1cef",
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
              "id": "f2f26c8b-e6d5-45e1-aa08-7568ab0de7a6"
            }
          ]
        },
        {
          "id": "a2bf50af-8943-48c9-8100-d1caf85ba55d",
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
              "id": "58c296b9-b8c9-406e-918a-707ed971a4ba"
            }
          ]
        },
        {
          "id": "979d6d84-b516-485f-94b2-d3e5e28c39b3",
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
              "id": "a9e1f637-8a22-40e8-b6ce-1a2836f4ecde"
            }
          ]
        },
        {
          "id": "42e28966-1e58-46f7-a068-011cdd81581a",
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
              "id": "33568d8a-3859-40f2-8487-cd4a388786fc"
            }
          ]
        },
        {
          "id": "4b4e266f-3f14-4dab-9e34-0c6d707a8b79",
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
              "id": "63ab01e6-641d-4c32-bd78-0087c8ce68fe"
            }
          ]
        },
        {
          "id": "9a6d09b8-8617-4065-884e-f64b08b511d6",
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
              "id": "abe8139c-d30a-44f3-a4dd-a7f66b6d1fea"
            }
          ]
        },
        {
          "id": "f0183563-8124-499a-8ef3-cc1e5a821ca6",
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
              "id": "64d32cf5-9585-4806-8625-b794d0164948"
            }
          ]
        },
        {
          "id": "15687934-2fc5-41ec-8fbf-0e49c10f2e68",
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
              "id": "0592fd95-3069-43d0-9dca-0124fdcce970"
            }
          ]
        },
        {
          "id": "4ecb7649-f67c-4d97-9682-325bfe41157d",
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
              "id": "089af218-9163-4ca3-8bf3-bef7d8e6e770"
            }
          ]
        },
        {
          "id": "9ef7c834-eeec-4dc7-94cf-9e7907eeb8fe",
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
              "id": "85797695-ef32-44a2-a1d1-5974e4edfdf3"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "0e90886d-7d4b-479c-9da1-2b74ef2d0586",
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
              "id": "4b4969a5-00d9-472c-85ba-ab935b880dea"
            }
          ]
        },
        {
          "id": "87717ee8-aa2d-4907-8b16-6db88c869d3e",
          "name": "getUser",
          "request": {
            "url": "http://example.com/api/user",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the current user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e85aa798-72ad-4b14-abcb-97a40ff6f850"
            }
          ]
        },
        {
          "id": "7b86a26a-e3e3-4be5-aa33-6da84dfc0cd0",
          "name": "getUserUnreadItems",
          "request": {
            "url": "http://example.com/api/user/:userId/rooms/:roomId/unreadItems",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "You can retrieve unread items and mentions using the following endpoint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e17cb6e-8f07-45a2-8749-4dff07fe0bb3"
            }
          ]
        }
      ]
    }
  ]
}