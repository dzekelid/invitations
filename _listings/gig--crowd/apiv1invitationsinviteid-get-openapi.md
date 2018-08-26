---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Get Invitations Inviteid
  version: 1.0.0
  description: Get invitations inviteid.
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