{
  "info": {
    "name": "Gitter API Delete Room",
    "_postman_id": "762b7383-2a27-423a-8bfd-0fdf0d716aa7",
    "description": "Deletes a room.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "ea9595bb-dba1-4985-bae8-bdee28302ac9",
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
              "id": "9cd89622-1b28-44e5-9465-84e2265c7083"
            }
          ]
        }
      ]
    },
    {
      "name": "Rooms",
      "item": [
        {
          "id": "27439e54-638d-424d-9541-7958076f3db1",
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
              "id": "bc0ddbfd-4a21-4fcc-8fad-216a23ba5088"
            }
          ]
        },
        {
          "id": "24f24fdc-2bbf-4166-be18-87e06cbdf35b",
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
              "id": "2cc40683-33cd-4aab-9e08-98f76199ac6d"
            }
          ]
        },
        {
          "id": "bf3d698e-8456-475e-8fe5-f3fb6a047117",
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
              "id": "8cec577f-4380-4162-8faa-948b0c1feb29"
            }
          ]
        },
        {
          "id": "b7467657-bded-4742-88a5-0ae8897b0206",
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
              "id": "82407e0f-6e63-490e-bdc5-1a1d33c2b0d6"
            }
          ]
        },
        {
          "id": "00316a64-5b1f-4ea4-b9a3-cda8944f1b89",
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
              "id": "ea23f693-c0c9-4fe8-89de-c5f3201217cd"
            }
          ]
        }
      ]
    }
  ]
}