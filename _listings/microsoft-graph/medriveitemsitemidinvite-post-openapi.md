---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Send A Sharing Invitation
  description: Send a sharing invitation Sends a sharing invitation for a DriveItem.
    A sharing invitation provides permissions to the recipients and optionally sends
    an email to the recipients to notify them the item was shared.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/drive/items/{item-id}/invite:
    post:
      summary: Send A Sharing Invitation
      description: Send a sharing invitation Sends a sharing invitation for a DriveItem.
        A sharing invitation provides permissions to the recipients and optionally
        sends an email to the recipients to notify them the item was shared.
      operationId: SendASharingInvitation
      x-api-path-slug: medriveitemsitemidinvite-post
      parameters:
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - SendSharing
      - Invitation
  /drive/items/{item-id}/invite:
    post:
      summary: Send A Sharing Invitation
      description: Send a sharing invitation Sends a sharing invitation for a DriveItem.
        A sharing invitation provides permissions to the recipients and optionally
        sends an email to the recipients to notify them the item was shared.
      operationId: SendASharingInvitation
      x-api-path-slug: driveitemsitemidinvite-post
      parameters:
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - SendSharing
      - Invitation
  /drives/{drive-id}/items/{item-id}/invite:
    post:
      summary: Send A Sharing Invitation
      description: Send a sharing invitation Sends a sharing invitation for a DriveItem.
        A sharing invitation provides permissions to the recipients and optionally
        sends an email to the recipients to notify them the item was shared.
      operationId: SendASharingInvitation
      x-api-path-slug: drivesdriveiditemsitemidinvite-post
      parameters:
      - in: path
        name: drive-id
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - SendSharing
      - Invitation
  /groups/{group-id}/drive/items/{item-id}/invite:
    post:
      summary: Send A Sharing Invitation
      description: Send a sharing invitation Sends a sharing invitation for a DriveItem.
        A sharing invitation provides permissions to the recipients and optionally
        sends an email to the recipients to notify them the item was shared.
      operationId: SendASharingInvitation
      x-api-path-slug: groupsgroupiddriveitemsitemidinvite-post
      parameters:
      - in: path
        name: group-id
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - SendSharing
      - Invitation
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