swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 1
info:
  title: GoToWebinar API
  description: todo-add-description
  version: 1.0.0
host: api.getgo.com
basePath: /G2W/rest/organizers
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{organizerKey}/webinars/{webinarKey}/panelists/{panelistKey}/resendInvitation:
    post:
      summary: Resend panelist invitation
      description: Resend panelist invitation.
      operationId: WebinarsPanelistsPanelistKeyResendInvitationByOrganizerKeyAndWebinarKeyPost
      x-api-path-slug: organizerkeywebinarswebinarkeypanelistspanelistkeyresendinvitation-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: panelistKey
      - in: path
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Resend
      - Panelist
      - Invitation
  /{organizerKey}/webinars/{webinarKey}/coorganizers/{coorganizerkey}/resendInvitation:
    post:
      summary: Resend invitation
      description: Resend invitation.
      operationId: WebinarsCoorganizersCoorganizerkeyResendInvitationByOrganizerKeyAndWebinarKeyPost
      x-api-path-slug: organizerkeywebinarswebinarkeycoorganizerscoorganizerkeyresendinvitation-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: coorganizerkey
      - in: path
        name: organizerKey
      - in: path
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Resend
      - Invitation