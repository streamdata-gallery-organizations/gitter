{
  "info": {
    "name": "Gitter API List rooms",
    "_postman_id": "2755a552-e721-4ccd-8806-36795d13a0ff",
    "description": "List rooms the current user is in.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "4b503d49-7e7d-466d-b429-15750ba15d8b",
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
              "id": "97649b85-824c-47fe-8f48-33964436c508"
            }
          ]
        }
      ]
    },
    {
      "name": "Rooms",
      "item": [
        {
          "id": "f06846f0-c824-4aa3-8ab5-b8a6a7c23fd4",
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
              "id": "6db4c9cc-6850-4d9c-ac5e-59a1f6205357"
            }
          ]
        }
      ]
    }
  ]
}