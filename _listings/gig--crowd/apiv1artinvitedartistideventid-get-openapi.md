---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Get Art Invited Artistid Eventid
  version: 1.0.0
  description: Get art invited artistid eventid.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/invitations/{inviteId}:
    get:
      summary: Get Invitations Inviteid
      description: Get invitations inviteid.
      operationId: getApiV1InvitationsInvite
      x-api-path-slug: apiv1invitationsinviteid-get
      parameters:
      - in: path
        name: inviteId
      responses:
        200:
          description: OK
      tags:
      - Invitations
      - Inviteid
  /api/v1/account/register/invite:
    post:
      summary: Post Account Register Invite
      description: Post account register invite.
      operationId: postApiV1AccountRegisterInvite
      x-api-path-slug: apiv1accountregisterinvite-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
      - Register
      - Invite
  /api/v1/request/org/invite:
    post:
      summary: Post Request Org Invite
      description: Post request org invite.
      operationId: postApiV1RequestOrgInvite
      x-api-path-slug: apiv1requestorginvite-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Request
      - Org
      - Invite
  /api/v1/request/art/invite:
    post:
      summary: Post Request Art Invite
      description: Post request art invite.
      operationId: postApiV1RequestArtInvite
      x-api-path-slug: apiv1requestartinvite-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Request
      - Art
      - Invite
  /api/v1/art/invited/{artistId}/{eventId}:
    get:
      summary: Get Art Invited Artistid Eventid
      description: Get art invited artistid eventid.
      operationId: getApiV1ArtInvitedArtistEvent
      x-api-path-slug: apiv1artinvitedartistideventid-get
      parameters:
      - in: path
        name: artistId
      - in: path
        name: eventId
      responses:
        200:
          description: OK
      tags:
      - Art
      - Invited
      - Artistid
      - Eventid
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