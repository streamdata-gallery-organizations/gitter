{
  "info": {
    "name": "Gitter API User Repos",
    "_postman_id": "d4c93bcf-07e3-4cab-a95b-9c5416cbd240",
    "description": "List of the user's GitHub Repositories and their respective Room if available.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "8e8d9d7d-b37e-4871-bde2-e99903f0967e",
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
              "id": "5e2a348a-d7f8-4d02-92f7-99e4c61a06f9"
            }
          ]
        },
        {
          "id": "62bd3cd9-d839-4c82-ac2e-9ef25d06eac2",
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
              "id": "cbba1e01-2d92-4cad-8f1f-e11aa2dd45bd"
            }
          ]
        }
      ]
    },
    {
      "name": "Rooms",
      "item": [
        {
          "id": "bb6b4372-8946-4ba6-af03-054fc89de312",
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
              "id": "7a85fa56-7bfe-4b5e-bc6d-fdc6c0c761d9"
            }
          ]
        },
        {
          "id": "83939cdf-033e-4fa0-be4d-fbb4930019eb",
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
              "id": "fc5ae6d1-fd59-4b3b-9e77-fadce1e02fc9"
            }
          ]
        },
        {
          "id": "cc8f972c-0562-4849-a31c-07fc582c3e6e",
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
              "id": "661ca66c-20b4-48a2-a637-6affb65406ca"
            }
          ]
        },
        {
          "id": "69cd14e4-cbe7-4781-8f6d-cc3a3f4429e7",
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
              "id": "89c5fd67-a501-41be-819c-e479ae6336e9"
            }
          ]
        },
        {
          "id": "b63646f0-8d0f-4a3b-8d92-fae99a07e22b",
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
              "id": "23499bc5-1ba9-4d54-8c34-f63ce331cdd2"
            }
          ]
        },
        {
          "id": "303564d0-61e9-4bd4-bd90-572a7b051844",
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
              "id": "2e14d4d2-988d-4275-9fdb-d0fbf53bd811"
            }
          ]
        },
        {
          "id": "976ff67a-2b45-487d-91d9-17f4e13ea2f4",
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
              "id": "274cc057-ced8-4197-86d1-a70f843ff337"
            }
          ]
        },
        {
          "id": "52d47130-647a-4966-b964-ecef000f49d7",
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
              "id": "f9e1cf39-3256-434a-8c57-8bd3dc492142"
            }
          ]
        },
        {
          "id": "6370689c-d89d-4a3c-9c6c-6571ebdf3e36",
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
              "id": "40717b07-81c8-4eb5-a78d-d50c732440cc"
            }
          ]
        },
        {
          "id": "a5d7b946-3f72-4838-94b9-ce0bc3ed799b",
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
              "id": "e85d4b65-1a50-4084-a04f-cc301ffe72a6"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "318cb4c4-5803-4e91-ae8c-d0c1dad27a7b",
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
              "id": "640c0396-4e45-47e0-b9dd-0633c5720d60"
            }
          ]
        },
        {
          "id": "264d7618-fd90-4bfc-bb33-3335431c783e",
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
              "id": "267894f8-a79b-41c6-9630-72b0b3ef4388"
            }
          ]
        },
        {
          "id": "96fa3377-3fcf-4c4b-a275-1232e567f421",
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
              "id": "d5c8414e-ee00-46c9-9348-ae96e85952cb"
            }
          ]
        },
        {
          "id": "85859d37-902a-4621-abba-06f14e1fb743",
          "name": "getUserOrgs",
          "request": {
            "url": "http://example.com/api/user/:userId/orgs",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of the user's GitHub Organisations and their respective Room if available."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cbe44edc-14c6-492e-8068-b624d24e234d"
            }
          ]
        },
        {
          "id": "84a6b21a-84a2-4048-b5d1-e5291086fc9f",
          "name": "getUserRepos",
          "request": {
            "url": "http://example.com/api/user/:userId/repos",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of the user's GitHub Repositories and their respective Room if available."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7851dac2-3696-49b5-9135-0d06a64ba85f"
            }
          ]
        }
      ]
    },
    {
      "name": "Messages",
      "item": [
        {
          "id": "257323df-b32a-4f5f-b8a5-b3d528318431",
          "name": "markUnreadItemsasRead",
          "request": {
            "url": "http://example.com/api/user/:userId/rooms/:roomId/unreadItems?chat=chat",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "There is an additional endpoint nested under rooms that you can use to mark chat messages as read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "208fb4cd-9bac-40a9-be72-e917776f05ab"
            }
          ]
        }
      ]
    }
  ]
}