---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box Get status of the invite
  description: ""
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /invites/{INVITE_ID}:
    get:
      summary: Get status of the invite
      description: ""
      operationId: getInvite
      x-api-path-slug: invitesinvite-id-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: INVITE_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Invites
      - Invite
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