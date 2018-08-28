---
name: Google Classroom
x-slug: google-classroom
description: Google Classroom is mission control for your classes. As a free service
  for teachers and students, you can create classes, distribute assignments, send
  feedback, and see everything in one place. Instant. Paperless. Easy.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Invitations
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/apis.md
specificationVersion: "0.14"
apis:
- name: Google Classroom - Get Invitations
  x-api-slug: v1invitations-get
  description: |-
    Returns a list of invitations that the requesting user is permitted to
    view, restricted to those that match the list request.

    *Note:* At least one of `user_id` or `course_id` must be supplied. Both
    fields can be supplied.

    This method returns the following error codes:

    * `PERMISSION_DENIED` for access errors.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitations-get-openapi.md
- name: Google Classroom - Create Invitation
  x-api-slug: v1invitations-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitations-post-openapi.md
- name: Google Classroom - Delete Invitation
  x-api-slug: v1invitationsid-delete
  description: |-
    Deletes an invitation.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to delete the
    requested invitation or for access errors.
    * `NOT_FOUND` if no invitation exists with the requested ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitationsid-delete-openapi.md
- name: Google Classroom - Get Invitation
  x-api-slug: v1invitationsid-get
  description: |-
    Returns an invitation.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to view the
    requested invitation or for access errors.
    * `NOT_FOUND` if no invitation exists with the requested ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitationsid-get-openapi.md
- name: Google Classroom - Accept Invitation
  x-api-slug: v1invitationsidaccept-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitationsidaccept-post-openapi.md
- name: Google Classroom - Get Invitations
  x-api-slug: v1invitations-get
  description: |-
    Returns a list of invitations that the requesting user is permitted to
    view, restricted to those that match the list request.

    *Note:* At least one of `user_id` or `course_id` must be supplied. Both
    fields can be supplied.

    This method returns the following error codes:

    * `PERMISSION_DENIED` for access errors.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitations-get-openapi.md
- name: Google Classroom - Get Invitations
  x-api-slug: v1invitations-get
  description: |-
    Returns a list of invitations that the requesting user is permitted to
    view, restricted to those that match the list request.

    *Note:* At least one of `user_id` or `course_id` must be supplied. Both
    fields can be supplied.

    This method returns the following error codes:

    * `PERMISSION_DENIED` for access errors.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitations-get-openapi.md
- name: Google Classroom - Create Invitation
  x-api-slug: v1invitations-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitations-post-openapi.md
- name: Google Classroom - Create Invitation
  x-api-slug: v1invitations-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitations-post-openapi.md
- name: Google Classroom - Create Invitation
  x-api-slug: v1invitations-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitations-post-openapi.md
- name: Google Classroom - Delete Invitation
  x-api-slug: v1invitationsid-delete
  description: |-
    Deletes an invitation.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to delete the
    requested invitation or for access errors.
    * `NOT_FOUND` if no invitation exists with the requested ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitationsid-delete-openapi.md
- name: Google Classroom - Delete Invitation
  x-api-slug: v1invitationsid-delete
  description: |-
    Deletes an invitation.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to delete the
    requested invitation or for access errors.
    * `NOT_FOUND` if no invitation exists with the requested ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitationsid-delete-openapi.md
- name: Google Classroom - Delete Invitation
  x-api-slug: v1invitationsid-delete
  description: |-
    Deletes an invitation.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to delete the
    requested invitation or for access errors.
    * `NOT_FOUND` if no invitation exists with the requested ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitationsid-delete-openapi.md
- name: Google Classroom - Get Invitation
  x-api-slug: v1invitationsid-get
  description: |-
    Returns an invitation.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to view the
    requested invitation or for access errors.
    * `NOT_FOUND` if no invitation exists with the requested ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitationsid-get-openapi.md
- name: Google Classroom - Get Invitation
  x-api-slug: v1invitationsid-get
  description: |-
    Returns an invitation.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to view the
    requested invitation or for access errors.
    * `NOT_FOUND` if no invitation exists with the requested ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitationsid-get-openapi.md
- name: Google Classroom - Get Invitation
  x-api-slug: v1invitationsid-get
  description: |-
    Returns an invitation.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to view the
    requested invitation or for access errors.
    * `NOT_FOUND` if no invitation exists with the requested ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitationsid-get-openapi.md
- name: Google Classroom - Accept Invitation
  x-api-slug: v1invitationsidaccept-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitationsidaccept-post-openapi.md
- name: Google Classroom - Accept Invitation
  x-api-slug: v1invitationsidaccept-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitationsidaccept-post-openapi.md
- name: Google Classroom - Accept Invitation
  x-api-slug: v1invitationsidaccept-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitationsidaccept-post-openapi.md
- name: Google Classroom - Get Invitations
  x-api-slug: v1invitations-get
  description: |-
    Returns a list of invitations that the requesting user is permitted to
    view, restricted to those that match the list request.

    *Note:* At least one of `user_id` or `course_id` must be supplied. Both
    fields can be supplied.

    This method returns the following error codes:

    * `PERMISSION_DENIED` for access errors.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitations-get-openapi.md
- name: Google Classroom - Create Invitation
  x-api-slug: v1invitations-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitations-post-openapi.md
- name: Google Classroom - Delete Invitation
  x-api-slug: v1invitationsid-delete
  description: |-
    Deletes an invitation.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to delete the
    requested invitation or for access errors.
    * `NOT_FOUND` if no invitation exists with the requested ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitationsid-delete-openapi.md
- name: Google Classroom - Get Invitation
  x-api-slug: v1invitationsid-get
  description: |-
    Returns an invitation.

    This method returns the following error codes:

    * `PERMISSION_DENIED` if the requesting user is not permitted to view the
    requested invitation or for access errors.
    * `NOT_FOUND` if no invitation exists with the requested ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitationsid-get-openapi.md
- name: Google Classroom - Accept Invitation
  x-api-slug: v1invitationsidaccept-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-classroom.png
  humanURL: https://classroom.google.com/
  baseURL: ://classroom.googleapis.com//
  tags: Education, Google APIs, Stack Network, API Service Provider, API Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/invitations/master/_listings/google-classroom/v1invitationsidaccept-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.civic.information.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.classroom.stack.network
- type: x-button
  url: https://developers.google.com/classroom/guides/sharebutton
- type: x-developer
  url: https://developers.google.com/classroom/
- type: x-getting-started
  url: ""
- type: x-issues
  url: https://code.google.com/a/google.com/p/apps-api-issues/issues/list?can=2&q=label%3AAPI-Classroom
- type: x-website
  url: https://classroom.google.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---