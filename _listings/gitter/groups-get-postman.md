{
  "info": {
    "name": "Gitter API List Groups",
    "_postman_id": "5d345c6c-ec7a-4a5a-8378-f50552070da0",
    "description": "List groups the current user is in.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "3e6df0d7-b3d1-457d-9e5d-e7cb8bb018d8",
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
              "id": "d0817b80-b3e2-4847-9f69-8d4a095db77d"
            }
          ]
        }
      ]
    }
  ]
}