{
  "info": {
    "name": "Gitter API Group Rooms",
    "_postman_id": "e02f32a4-2228-4099-a80e-8836e3cc88a8",
    "description": "List rooms under group",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "156b5658-969c-401a-875f-a400c2eb8c1b",
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
              "id": "252de3db-d9fe-499e-a40a-9ed518ad980e"
            }
          ]
        }
      ]
    }
  ]
}