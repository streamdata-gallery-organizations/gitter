---
swagger: "2.0"
x-collection-name: Gitter
x-complete: 0
info:
  title: Gitter API Delete Room
  version: 1.0.0
  description: Deletes a room.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups:
    get:
      summary: List Groups
      description: List groups the current user is in.
      operationId: listGroups
      x-api-path-slug: groups-get
      responses:
        200:
          description: OK
      tags:
      - Groups
  /groups/:groupId/rooms:
    get:
      summary: Group Rooms
      description: List rooms under group
      operationId: getGroupRooms
      x-api-path-slug: groupsgroupidrooms-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Rooms
  /rooms:
    get:
      summary: List rooms
      description: List rooms the current user is in.
      operationId: listRooms
      x-api-path-slug: rooms-get
      responses:
        200:
          description: OK
      tags:
      - Rooms
  /user/:userId/rooms:
    post:
      summary: Join Room
      description: To join a room you'll need to provide a URI for it. Said URI can
        represent a GitHub Org, a GitHub Repo or a Gitter Channel.
      operationId: joinRoom
      x-api-path-slug: useruseridrooms-post
      responses:
        200:
          description: OK
      tags:
      - Rooms
  /rooms/:room_id/users/:user_id:
    get:
      summary: Remove Room
      description: Remove a user from a room.
      operationId: removeRoom
      x-api-path-slug: roomsroom-idusersuser-id-get
      responses:
        200:
          description: OK
      tags:
      - Rooms
  /rooms/:roomId:
    put:
      summary: Update room
      description: Updates a room.
      operationId: updateRoom
      x-api-path-slug: roomsroomid-put
      parameters:
      - in: query
        name: noindex
        description: Whether the room is indexed by search engines
        type: string
        format: string
      - in: query
        name: tags
        description: Tags that define the room
        type: string
        format: string
      - in: query
        name: topic
        description: Room topic
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Rooms
    delete:
      summary: Delete Room
      description: Deletes a room.
      operationId: deleteRoom
      x-api-path-slug: roomsroomid-delete
      responses:
        200:
          description: OK
      tags:
      - Rooms
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---