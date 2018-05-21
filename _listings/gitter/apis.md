---
name: Gitter
x-slug: gitter
description: Gitter is a chat and networking platform that helps to manage, grow and
  connect communities through messaging, content and discovery.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
x-kinRank: "8"
x-alexaRank: "18282"
tags: Gitter
created: "2018-05-21"
modified: "2018-05-21"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/apis.md
specificationVersion: "0.14"
apis:
- name: Gitter API List Groups
  x-api-slug: gitter-api
  description: List groups the current user is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///groups
  tags: Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/groups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/groups-get-openapi.md
- name: Gitter API Group Rooms
  x-api-slug: gitter-api
  description: List rooms under group
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///groups/:groupId/rooms
  tags: Groups,Rooms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/groupsgroupidrooms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/groupsgroupidrooms-get-openapi.md
- name: Gitter API List rooms
  x-api-slug: gitter-api
  description: List rooms the current user is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///rooms
  tags: Rooms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/rooms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/rooms-get-openapi.md
- name: Gitter API Join Room
  x-api-slug: gitter-api
  description: To join a room you'll need to provide a URI for it. Said URI can represent
    a GitHub Org, a GitHub Repo or a Gitter Channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///user/:userId/rooms
  tags: Rooms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/useruseridrooms-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/useruseridrooms-post-openapi.md
- name: Gitter API Remove Room
  x-api-slug: gitter-api
  description: Remove a user from a room.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///rooms/:room_id/users/:user_id
  tags: Rooms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/roomsroom-idusersuser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/roomsroom-idusersuser-id-get-openapi.md
- name: Gitter API Update room
  x-api-slug: gitter-api
  description: Updates a room.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///rooms/:roomId
  tags: Rooms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/roomsroomid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/roomsroomid-put-openapi.md
- name: Gitter API Delete Room
  x-api-slug: gitter-api
  description: Deletes a room.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///rooms/:roomId
  tags: Rooms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/roomsroomid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/roomsroomid-delete-openapi.md
- name: Gitter API Room Users
  x-api-slug: gitter-api
  description: List of Users currently in the room.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///rooms/:roomId/users
  tags: Rooms,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/roomsroomidusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/roomsroomidusers-get-openapi.md
- name: Gitter API List Room Messages
  x-api-slug: gitter-api
  description: List of messages in a room.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///rooms/:roomId/chatMessages
  tags: Rooms, Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/roomsroomidchatmessages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/roomsroomidchatmessages-get-openapi.md
- name: Gitter API Get Room Message
  x-api-slug: gitter-api
  description: There is also a way to retrieve a single message using its id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///rooms/:roomId/chatMessages/:messageId
  tags: Rooms,Message
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/roomsroomidchatmessagesmessageid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/roomsroomidchatmessagesmessageid-get-openapi.md
- name: Gitter API Send Message
  x-api-slug: gitter-api
  description: Send a message to a room.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///rooms/:roomId/chatMessages
  tags: Rooms,Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/roomsroomidchatmessages-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/roomsroomidchatmessages-post-openapi.md
- name: Gitter API Update Message
  x-api-slug: gitter-api
  description: Update a message.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///rooms/:roomId/chatMessages/:chatMessageId
  tags: Rooms,Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/roomsroomidchatmessageschatmessageid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/roomsroomidchatmessageschatmessageid-put-openapi.md
- name: Gitter API Get User
  x-api-slug: gitter-api
  description: Get the current user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///user
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/user-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/user-get-openapi.md
- name: Gitter API Get User Rooms
  x-api-slug: gitter-api
  description: List of Rooms the user is part of.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///user/:userId/rooms
  tags: Users,Rooms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/useruseridrooms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/useruseridrooms-get-openapi.md
- name: Gitter API Get User Unread Items
  x-api-slug: gitter-api
  description: You can retrieve unread items and mentions using the following endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///user/:userId/rooms/:roomId/unreadItems
  tags: Users,Messages,Unread
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/useruseridroomsroomidunreaditems-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/useruseridroomsroomidunreaditems-get-openapi.md
- name: Gitter API Mark Unread Items as Read
  x-api-slug: gitter-api
  description: There is an additional endpoint nested under rooms that you can use
    to mark chat messages as read.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///user/:userId/rooms/:roomId/unreadItems
  tags: Messages,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/useruseridroomsroomidunreaditems-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/useruseridroomsroomidunreaditems-post-openapi.md
- name: Gitter API User Orgs
  x-api-slug: gitter-api
  description: List of the user's GitHub Organisations and their respective Room if
    available.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///user/:userId/orgs
  tags: Users,Organizations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/useruseridorgs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/useruseridorgs-get-openapi.md
- name: Gitter API User Repos
  x-api-slug: gitter-api
  description: List of the user's GitHub Repositories and their respective Room if
    available.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///user/:userId/repos
  tags: Users,Repositories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/useruseridrepos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/useruseridrepos-get-openapi.md
- name: Gitter API Get User Channels
  x-api-slug: gitter-api
  description: List of Gitter channels nested under the current user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///user/:userId/channels
  tags: Users,Channels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/useruseridchannels-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/useruseridchannels-get-openapi.md
- name: Gitter API
  x-api-slug: gitter-api
  description: Gitter is a chat and networking platform that helps to manage, grow
    and connect communities through messaging, content and discovery.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https:///
  tags: Gitter
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/gitter/master/_listings/gitter/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/gitter
- type: x-developer
  url: https://developer.gitter.im/docs/streaming-api
- type: x-github
  url: https://github.com/gitterHQ
- type: x-curated-source
  url: https://gitter.im/apiaryio/api-blueprint
- type: x-website
  url: http://gitter.im
- type: x-twitter
  url: https://twitter.com/gitchat
- type: x-website
  url: https://gitter.im
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---