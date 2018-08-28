swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Utility APIs
  description: canvas-lms-includes-a-rest-api-for-accessing-and-modifying-data-externally-from-the-main-application-in-your-own-programs-and-scripts--
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