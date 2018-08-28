swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost
  version: 1.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /teams/members/invite:
    post:
      summary: Add user to team from invite
      description: |-
        Using either an invite id or hash/data pair from an email invite link, add a user to a team.
        ##### Permissions
        Must be authenticated.
      operationId: using-either-an-invite-id-or-hashdata-pair-from-an-email-invite-link-add-a-user-to-a-team-permission
      x-api-path-slug: teamsmembersinvite-post
      parameters:
      - in: query
        name: data
        description: Data with time and team id
      - in: query
        name: hash
        description: Hash value with time, team id and and InviteSaltId
      - in: query
        name: invite_id
        description: Invite id to add user to the team
      responses:
        200:
          description: OK
      tags:
      - User
      - To
      - Team
      - From
      - Invite
  /teams/{team_id}/invite/email:
    post:
      summary: Invite users to the team by email
      description: |-
        Invite users to the existing team usign the user's email.
        ##### Permissions
        Must have `invite_to_team` permission for the team.
      operationId: invite-users-to-the-existing-team-usign-the-users-email-permissionsmust-have-invite-to-team-permissi
      x-api-path-slug: teamsteam-idinviteemail-post
      parameters:
      - in: body
        name: body
        description: List of users email
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - Invite
      - Users
      - To
      - Team
      - By
      - Email
  /teams/invite/{invite_id}:
    get:
      summary: Get invite info for a team
      description: |-
        Get the `name`, `display_name`, `description` and `id` for a team from the invite id.

        __Minimum server version__: 4.0

        ##### Permissions
        No authentication required.
      operationId: get-the-name-display-name-description-and-id-for-a-team-from-the-invite-id-minimum-server-version--4
      x-api-path-slug: teamsinviteinvite-id-get
      parameters:
      - in: path
        name: invite_id
        description: Invite id for a team
      responses:
        200:
          description: OK
      tags:
      - Invite
      - Infoa
      - Team