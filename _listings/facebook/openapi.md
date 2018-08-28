swagger: "2.0"
x-collection-name: Facebook
x-complete: 1
info:
  title: Facebook
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{event}/invited:
    get:
      summary: Get Event Invited
      description: All of the users who have been invited to this event
      operationId: getEventInvited
      x-api-path-slug: eventinvited-get
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
      - Invited