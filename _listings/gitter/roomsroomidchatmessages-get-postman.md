{
  "info": {
    "name": "Gitter API List Room Messages",
    "_postman_id": "5e50db24-920d-418e-b268-97b606c92c09",
    "description": "List of messages in a room.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "a60a14b2-7124-4319-bb19-1b90b3c9bf24",
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
              "id": "3e20f043-d759-48b0-9e59-9b40ec9d4e00"
            }
          ]
        }
      ]
    },
    {
      "name": "Rooms",
      "item": [
        {
          "id": "1d53a820-d27c-4cfa-9576-7e8f4228a82e",
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
              "id": "080fa17f-f388-4224-9d0d-906debd38836"
            }
          ]
        },
        {
          "id": "77b4db88-8ca1-4ea6-aac4-ddfae71d7a97",
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
              "id": "63fd836b-832a-46a9-bc72-06ac4622b689"
            }
          ]
        },
        {
          "id": "710daf4a-bf47-4607-9cd8-dd9da8b37f4e",
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
              "id": "fe92578e-e952-4239-b0a5-0dc790b6fd2c"
            }
          ]
        },
        {
          "id": "e09e7a97-2fda-4a6c-8f55-548a439b55b5",
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
              "id": "d8f36db6-2d01-4e69-922d-b3c9f41f0499"
            }
          ]
        },
        {
          "id": "a632371d-41f4-4b43-b02e-6674be20257f",
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
              "id": "af5922dd-8bb7-4e38-a174-c6562be230c5"
            }
          ]
        },
        {
          "id": "bd6a3681-bd1c-4c17-9b94-9d2c6d38a5a7",
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
              "id": "5eb8fbf8-6435-47c9-98d5-f7d70286a9b0"
            }
          ]
        },
        {
          "id": "dccaac49-5605-48cf-83d5-cc87a6a90250",
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
              "id": "214d4286-7ddc-4ff3-8d1c-0b3b5c3a2cfa"
            }
          ]
        }
      ]
    }
  ]
}