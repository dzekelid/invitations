---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Groups API Invite others to a group
  description: Invite others to a group.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups/{group_id}/invite:
    post:
      summary: Invite others to a group
      description: Invite others to a group.
      operationId: invite-others-to-a-group
      x-api-path-slug: groupsgroup-idinvite-post
      parameters:
      - in: query
        name: invitees[]
        description: An array of email addresses to be sent invitations
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
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