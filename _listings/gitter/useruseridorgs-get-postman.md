{
  "info": {
    "name": "Gitter API User Orgs",
    "_postman_id": "8cc75ff5-36e7-456c-9646-36d21d22bd21",
    "description": "List of the user's GitHub Organisations and their respective Room if available.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "dabe99ac-f953-4924-aefe-8f5f4ba1576d",
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
              "id": "15982292-add2-482d-8ffa-b1631882bf4f"
            }
          ]
        },
        {
          "id": "ad97587e-5b9b-46de-8503-4dad1eca6d26",
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
              "id": "20fda6b4-68ae-4a23-955a-cec2499c4bf3"
            }
          ]
        }
      ]
    },
    {
      "name": "Rooms",
      "item": [
        {
          "id": "3e9a671a-ab48-4ffc-b0dd-72a20b5b90f2",
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
              "id": "cebc14b7-0ccd-4451-8ff4-29097abe7570"
            }
          ]
        },
        {
          "id": "09ab742c-1715-4728-b0d7-b6dda151bab2",
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
              "id": "0b30f96c-173f-4b28-84f3-3fc3aaa1c524"
            }
          ]
        },
        {
          "id": "eca637fe-495b-4b5c-a316-152323320e55",
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
              "id": "26fba9d7-1782-46fe-8b7d-fda886e68871"
            }
          ]
        },
        {
          "id": "47ccb0c5-ab70-4ce3-a859-ab5a9f56e7c5",
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
              "id": "24d0e154-c7cf-4b12-a6de-6cce7e9fb031"
            }
          ]
        },
        {
          "id": "e3cb3669-0045-4b66-b4f9-fe7c5708a171",
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
              "id": "84091706-fea4-47a6-ba73-a120c5e43344"
            }
          ]
        },
        {
          "id": "cc98f388-2ff1-4ae3-ae02-a534c0ab1ed4",
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
              "id": "59889dfa-9523-4ae5-b856-181a3b66822c"
            }
          ]
        },
        {
          "id": "937c9a89-ac41-4c1a-8c45-4d393cae5c0d",
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
              "id": "ede74fc1-a202-42c0-8a7d-c99e02e02fc6"
            }
          ]
        },
        {
          "id": "b7cb3c2d-bd03-4490-8c00-c1412474a52b",
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
              "id": "a13fa5cf-6ee6-4b47-9501-28594aa6ca40"
            }
          ]
        },
        {
          "id": "0c143ebe-f311-444f-b6c8-ec4adcd04baa",
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
              "id": "0213cf52-1164-42fe-8a67-d3c049050978"
            }
          ]
        },
        {
          "id": "f82cc535-1a7f-46a9-92dd-89db3dc23b6a",
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
              "id": "3b638d8c-6c77-4807-903b-2ba703ec10bf"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "fe21fbdc-263e-4ec6-a1f2-95ccdcc9c275",
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
              "id": "c2dbdbe3-0249-4b70-ba45-07cef6f9907b"
            }
          ]
        },
        {
          "id": "f042ccb0-bb45-4510-8112-671196f93b7a",
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
              "id": "b452e9e2-0aa0-4de7-8269-ab60cf91afed"
            }
          ]
        },
        {
          "id": "1ea563e5-a6f2-48bd-893a-350696a316b2",
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
              "id": "e89ce2f7-2584-4bdc-bcd6-f4fb9e6040bb"
            }
          ]
        },
        {
          "id": "f228a146-480f-4317-9a43-afc86b021511",
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
              "id": "42c7fe10-be92-4c00-8787-918e12265d38"
            }
          ]
        }
      ]
    },
    {
      "name": "Messages",
      "item": [
        {
          "id": "5bfa50dc-b7c2-4356-a2bd-0b39ed9ff72d",
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
              "id": "129cc8b5-c55e-408e-9326-2b90dc0dd7f0"
            }
          ]
        }
      ]
    }
  ]
}