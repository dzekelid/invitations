swagger: "2.0"
x-collection-name: Box
x-complete: 1
info:
  title: Box
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