swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
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