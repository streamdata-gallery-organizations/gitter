{
  "info": {
    "name": "Gitter API Room Users",
    "_postman_id": "48cc24e6-59cd-4417-a409-ac7c254d687a",
    "description": "List of Users currently in the room.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "dc69d436-0b60-4c83-a6da-eb6371c0d775",
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
              "id": "ecd06827-bb50-4000-8917-96ce045cee3d"
            }
          ]
        }
      ]
    },
    {
      "name": "Rooms",
      "item": [
        {
          "id": "14a9dd65-b466-44a1-beb9-e44ea87db7e0",
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
              "id": "5a09c0ec-871e-45b2-88e5-8e2fb8f7ef1f"
            }
          ]
        },
        {
          "id": "c373cf20-4c62-49e5-b683-58caae7b4ea1",
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
              "id": "4cadff27-7322-4286-8445-538e39f22658"
            }
          ]
        },
        {
          "id": "24293dc9-b4ca-4491-b515-7db6c89f6cf1",
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
              "id": "6a432e94-cd2b-40c5-ac1c-53ad058df31d"
            }
          ]
        },
        {
          "id": "0e2b423b-7635-42e0-a30a-2debfbaa772d",
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
              "id": "e029fb82-a51b-4341-8019-7f32bb4fb356"
            }
          ]
        },
        {
          "id": "54ef5f4e-2856-441d-b6c7-f990808e1fa1",
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
              "id": "105eec2c-66e0-4106-8749-c1a03f8c48d1"
            }
          ]
        },
        {
          "id": "7972edc1-0035-459d-86d9-be4e49aa5a60",
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
              "id": "00822613-98d0-48d0-9f3f-92263f600296"
            }
          ]
        }
      ]
    }
  ]
}