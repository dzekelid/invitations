swagger: "2.0"
x-collection-name: Reddit
x-complete: 1
info:
  title: Reddit
  version: 1.0.0
host: www.reddit.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  '{/r/subreddit}/accept_moderator_invite':
    post&nbsp;:
      summary: Add Subreddit Accept Moderator Invite
      description: Accept an invite to moderate the specified subreddit.
      operationId: post&nbsp;RSubredditAcceptModeratorInvite
      x-api-path-slug: rsubredditaccept-moderator-invite-postnbsp
      parameters:
      - in: query
        name: api_type
        description: the string json
        type: string
      - in: query
        name: uh / X-Modhash header
        description: a modhash
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subreddit
      - Accept
      - Moderator
      - Invite