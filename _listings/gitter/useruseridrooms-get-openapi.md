---
swagger: "2.0"
x-collection-name: Gitter
x-complete: 0
info:
  title: Gitter API Get User Rooms
  version: 1.0.0
  description: List of Rooms the user is part of.
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
    get:
      summary: Get User Rooms
      description: List of Rooms the user is part of.
      operationId: getUserRooms
      x-api-path-slug: useruseridrooms-get
      responses:
        200:
          description: OK
      tags:
      - Users
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
  /rooms/:roomId/users:
    get:
      summary: Room Users
      description: List of Users currently in the room.
      operationId: getRoomUsers
      x-api-path-slug: roomsroomidusers-get
      parameters:
      - in: query
        name: limit
        description: maximum number of users to return (default 30)
        type: string
        format: string
      - in: query
        name: q
        description: Search query
        type: string
        format: string
      - in: query
        name: skip
        description: Skip n users
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Rooms
      - Users
  /rooms/:roomId/chatMessages:
    get:
      summary: List Room Messages
      description: List of messages in a room.
      operationId: listRoomMessages
      x-api-path-slug: roomsroomidchatmessages-get
      parameters:
      - in: query
        name: afterId
        description: Get messages after afterId
        type: string
        format: string
      - in: query
        name: aroundId
        description: Get messages around aroundId including this message
        type: string
        format: string
      - in: query
        name: beforeId
        description: Get messages before beforeId
        type: string
        format: string
      - in: query
        name: limit
        description: Maximum number of messages to return (constrained to 100 or less)
        type: string
        format: string
      - in: query
        name: q
        description: Search query
        type: string
        format: string
      - in: query
        name: skip
        description: Skip n messages (constrained to 5000 or less)
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Rooms
      - Messages
    post:
      summary: Send Message
      description: Send a message to a room.
      operationId: sendMessage
      x-api-path-slug: roomsroomidchatmessages-post
      parameters:
      - in: query
        name: text
        description: Required Body of the message
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Rooms
      - Messages
  /rooms/:roomId/chatMessages/:messageId:
    get:
      summary: Get Room Message
      description: There is also a way to retrieve a single message using its id.
      operationId: getRoomMessage
      x-api-path-slug: roomsroomidchatmessagesmessageid-get
      responses:
        200:
          description: OK
      tags:
      - Rooms
      - Message
  /rooms/:roomId/chatMessages/:chatMessageId:
    put:
      summary: Update Message
      description: Update a message.
      operationId: updateMessage
      x-api-path-slug: roomsroomidchatmessageschatmessageid-put
      parameters:
      - in: query
        name: text
        description: Required Body of the message
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Rooms
      - Messages
  /user:
    get:
      summary: Get User
      description: Get the current user.
      operationId: getUser
      x-api-path-slug: user-get
      responses:
        200:
          description: OK
      tags:
      - Users
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