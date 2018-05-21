{
  "info": {
    "name": "Gitter API Get User",
    "_postman_id": "94a02655-cd57-40fe-b100-76857e06661b",
    "description": "Get the current user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "d81baa8a-6533-4e84-a83c-b865a8208ece",
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
              "id": "96cd17f3-d338-4c06-a728-cc526765a3d8"
            }
          ]
        },
        {
          "id": "a8d90535-87d3-4f46-b6eb-ad97826fcaee",
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
              "id": "5a323655-8242-43d4-aed5-8ff07ce290cd"
            }
          ]
        }
      ]
    },
    {
      "name": "Rooms",
      "item": [
        {
          "id": "d14e1398-129c-4bc8-a125-c4908005a447",
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
              "id": "22cb4b3d-b547-4a67-851c-0ff5adc8612e"
            }
          ]
        },
        {
          "id": "f92c8f5a-7de2-49e0-9f8b-4bdabb7c044e",
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
              "id": "9e0a4496-a64c-4a61-a26c-7e311541001a"
            }
          ]
        },
        {
          "id": "6d90125a-e19e-41ff-ba17-ee82179139fc",
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
              "id": "de4a1b14-bdf7-4c68-851c-1842a3682100"
            }
          ]
        },
        {
          "id": "e93957f0-778e-40ba-a26e-2d0472581c4b",
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
              "id": "c8915d9a-d697-44ea-be76-f117c462b174"
            }
          ]
        },
        {
          "id": "b054ab8c-441c-44fb-8efc-475017269bea",
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
              "id": "b59a2b1f-2575-4316-a95b-087b19a069e7"
            }
          ]
        },
        {
          "id": "3511b9e3-d326-4083-b881-bd38bad54629",
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
              "id": "64b24380-621b-4f1e-939b-5c40755e821a"
            }
          ]
        },
        {
          "id": "a67b906a-bd0f-4d7b-ac6a-3f4005cbbf47",
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
              "id": "03ec06ae-0738-4e9f-90dc-39ce22df8dc1"
            }
          ]
        },
        {
          "id": "c3491bcf-8723-4c8c-b795-c5b689c9f168",
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
              "id": "76073bf2-abe3-445f-8054-8ff2097916e1"
            }
          ]
        },
        {
          "id": "27bf133d-6cf5-4216-ac9b-8e4523a4270f",
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
              "id": "256c8152-0bee-48ac-b9c0-ef5cf90d936c"
            }
          ]
        },
        {
          "id": "9b466307-a17a-4819-a52a-59c09ec8118f",
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
              "id": "38528037-b6b5-486f-9d43-32f7d14ed05e"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "6e25630b-4023-4a6d-aaa5-bd4deaaf69d8",
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
              "id": "88ca78b9-3a80-4b40-b680-94aff1d947d3"
            }
          ]
        }
      ]
    }
  ]
}