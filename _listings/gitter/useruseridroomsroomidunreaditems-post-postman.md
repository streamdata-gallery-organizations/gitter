{
  "info": {
    "name": "Gitter API Mark Unread Items as Read",
    "_postman_id": "ede2007f-daa0-4402-b115-dbf782e0ba62",
    "description": "There is an additional endpoint nested under rooms that you can use to mark chat messages as read.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "78f4b7aa-c453-483c-b6cc-ac38c14e4549",
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
              "id": "d71fbc36-31fa-4f08-9100-63262597f387"
            }
          ]
        },
        {
          "id": "48be6b8f-1e12-499e-a920-4c3d6918618a",
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
              "id": "1acddd7b-7341-4c0f-ab07-e855b9b843f8"
            }
          ]
        }
      ]
    },
    {
      "name": "Rooms",
      "item": [
        {
          "id": "a1b9be70-673a-47ab-aef2-c8afbbe9edd8",
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
              "id": "26db514d-d3d2-496a-be98-5e609795d3fb"
            }
          ]
        },
        {
          "id": "e9f85fdc-5487-4c55-81ba-c927f09f2a2e",
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
              "id": "2bf45ca3-5a4e-4648-91d6-32e74a0c7d76"
            }
          ]
        },
        {
          "id": "8d07cf8e-13a1-446b-9a93-fc2210a6ca23",
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
              "id": "d245029b-19ac-4e38-8299-3aaebb9c0190"
            }
          ]
        },
        {
          "id": "1963f5a7-4e13-494f-b5b5-de288415b35e",
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
              "id": "03a74aab-7e7c-4e11-8dfa-44749fa6767a"
            }
          ]
        },
        {
          "id": "19c04f92-59ec-41fb-a548-0cb1e9150382",
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
              "id": "06dd7d7b-635e-4d1c-b1b8-35060a67c970"
            }
          ]
        },
        {
          "id": "578e31c4-e512-41bf-877f-65e1cae82b87",
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
              "id": "cdbf6dd9-8b9b-481e-8eae-e8ee783e648e"
            }
          ]
        },
        {
          "id": "09c2d2c7-0bd4-4166-a947-ca5c77c26f0b",
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
              "id": "72de23a6-2181-4509-a831-9084877fe07c"
            }
          ]
        },
        {
          "id": "305d9064-5293-4441-8caf-145d017ef630",
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
              "id": "4341da77-6ecc-4509-b7f1-9e8489712f14"
            }
          ]
        },
        {
          "id": "e403e57d-9594-410c-8683-7ca1c6751c50",
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
              "id": "ce3aa8cf-3de9-4023-ac03-5384acc7caf8"
            }
          ]
        },
        {
          "id": "cab8fe8f-bb64-4321-8545-3d679850dcb5",
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
              "id": "5dbabba5-6020-4910-925f-61e74b72496c"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "025f0369-55f7-49eb-a5b2-9f35073a5767",
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
              "id": "8bb499f3-a6ed-462d-9c31-4e2536f5430e"
            }
          ]
        },
        {
          "id": "23172296-8ba7-4655-986c-b2342844f99c",
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
              "id": "2ccefc83-c96b-4771-b505-fc6298930c30"
            }
          ]
        },
        {
          "id": "81b067ba-e64b-4f75-a1c4-f1274fc6394e",
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
              "id": "ff23fdb4-3877-42de-a3d5-296926ee2394"
            }
          ]
        }
      ]
    },
    {
      "name": "Messages",
      "item": [
        {
          "id": "14204510-c92b-481a-a9ef-60a98ff282f2",
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
              "id": "0ee012ed-a5a5-4b34-b839-837e87faff12"
            }
          ]
        }
      ]
    }
  ]
}