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
  /rooms/:roomId/chatMessages/:chatMessageId:
    put:
      summary: Update Message
      description: Update a message
      operationId: updateMessage
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
      - rooms
      - messages
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