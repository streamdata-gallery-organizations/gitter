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
  /user/:userId/rooms/:roomId/unreadItems:
    post:
      summary: Mark Unread Items as Read
      description: There is an additional endpoint nested under rooms that you can
        use to mark chat messages as read
      operationId: markUnreadItemsasRead
      parameters:
      - in: query
        name: chat
        description: Array of chatIds
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - messages
      - read
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