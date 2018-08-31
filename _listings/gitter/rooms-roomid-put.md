---
swagger: "2.0"
info:
  title: No Title
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rooms/:roomId:
    put:
      summary: Update room
      description: Updates a room
      operationId: updateRoom
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
      - rooms
definitions: []
x-collection-name: Gitter
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