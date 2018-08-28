---
swagger: "2.0"
x-collection-name: Google Classroom
x-complete: 0
info:
  title: Google Classroom API Get Invitation
  description: |-
    Returns an invitation.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to view the
    requested invitation or for access errors.
    * `NOT_FOUND` if no invitation exists with the requested ID.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: classroom.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/invitations:
    get:
      summary: Get Invitations
      description: |-
        Returns a list of invitations that the requesting user is permitted to
        view, restricted to those that match the list request.

        *Note:* At least one of `user_id` or `course_id` must be supplied. Both
        fields can be supplied.

        This method returns the following error codes:

        * `PERMISSION_DENIED` for access errors.
      operationId: classroom.invitations.list
      x-api-path-slug: v1invitations-get
      parameters:
      - in: query
        name: courseId
        description: Restricts returned invitations to those for a course with the
          specifiedidentifier
      - in: query
        name: pageSize
        description: Maximum number of items to return
      - in: query
        name: pageToken
        description: nextPageTokenvalue returned from a previouslist call, indicatingthat
          the subsequent page of results should be returned
      - in: query
        name: userId
        description: Restricts returned invitations to those for a specific user
      responses:
        200:
          description: OK
      tags:
      - Invitation
    post:
      summary: Create Invitation
      description: |-
        Creates an invitation. Only one invitation for a user and course may exist
        at a time. Delete and re-create an invitation to make changes.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to create
        invitations for this course or for access errors.
        * `NOT_FOUND` if the course or the user does not exist.
        * `FAILED_PRECONDITION` if the requested user's account is disabled or if
        the user already has this role or a role with greater permissions.
        * `ALREADY_EXISTS` if an invitation for the specified user and course
        already exists.
      operationId: classroom.invitations.create
      x-api-path-slug: v1invitations-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Invitation
  /v1/invitations/{id}:
    delete:
      summary: Delete Invitation
      description: |-
        Deletes an invitation.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to delete the
        requested invitation or for access errors.
        * `NOT_FOUND` if no invitation exists with the requested ID.
      operationId: classroom.invitations.delete
      x-api-path-slug: v1invitationsid-delete
      parameters:
      - in: path
        name: id
        description: Identifier of the invitation to delete
      responses:
        200:
          description: OK
      tags:
      - Invitation
    get:
      summary: Get Invitation
      description: |-
        Returns an invitation.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to view the
        requested invitation or for access errors.
        * `NOT_FOUND` if no invitation exists with the requested ID.
      operationId: classroom.invitations.get
      x-api-path-slug: v1invitationsid-get
      parameters:
      - in: path
        name: id
        description: Identifier of the invitation to return
      responses:
        200:
          description: OK
      tags:
      - Invitation
  /v1/invitations/{id}:accept:
    post:
      summary: Accept Invitation
      description: |-
        Accepts an invitation, removing it and adding the invited user to the
        teachers or students (as appropriate) of the specified course. Only the
        invited user may accept an invitation.

        This method returns the following error codes:

        * `PERMISSION_DENIED` if the requesting user is not permitted to accept the
        requested invitation or for access errors.
        * `FAILED_PRECONDITION` for the following request errors:
            * CourseMemberLimitReached
            * CourseNotModifiable
            * CourseTeacherLimitReached
            * UserGroupsMembershipLimitReached
        * `NOT_FOUND` if no invitation exists with the requested ID.
      operationId: classroom.invitations.accept
      x-api-path-slug: v1invitationsidaccept-post
      parameters:
      - in: path
        name: id
        description: Identifier of the invitation to accept
      responses:
        200:
          description: OK
      tags:
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