---
swagger: "2.0"
x-collection-name: uebermaps
x-complete: 0
info:
  title: uebermaps List your collaborator invitations
  description: List your collaborator invitations.
  termsOfService: https://uebermaps.com/terms/
  contact:
    name: uebermaps API Team
  version: "2.0"
host: uebermaps.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /collaborator_invitations:
    get:
      summary: List your collaborator invitations
      description: List your collaborator invitations.
      operationId: collaborator_invitations.get
      x-api-path-slug: collaborator-invitations-get
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Your
      - Collaborator
      - Invitations
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