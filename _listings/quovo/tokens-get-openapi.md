---
swagger: "2.0"
x-collection-name: Quovo
x-complete: 0
info:
  title: Quovo Get all active access tokens
  description: Retrieves all of your current Access Tokens.
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /connections/{connection_id}/sync:
    get:
      summary: Get a connection's sync progress
      description: Check the ongoing Sync progress of an Account.
      operationId: ConnectionsSyncByConnectionIdGet
      x-api-path-slug: connectionsconnection-idsync-get
      parameters:
      - in: path
        name: connection_id
      responses:
        200:
          description: OK
      tags:
      - Connections
      - Sync
      - Progress
    post:
      summary: Initiate a Sync on the Connection
      description: |-
        Initiates a new sync on the connection.

        Syncs are an ongoing update attempt on a connection. Syncing a newly created connection ensures the connction contains the most recent, available financial data, which includes current holdings and historical transactions.

        Before making the request, check that the `{{connection_id}}` Postman variable is set properly, or that the URL contains the correct connection id.

        The request will return a sync object with a `progress.state` of "queued", which indicates the sync request was sent successfully.
      operationId: ConnectionsSyncByConnectionIdPost5
      x-api-path-slug: connectionsconnection-idsync-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: connection_id
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Initiate
      - Sync
      - "On"
      - Connection
  /users/{user_id}/terms_of_use:
    get:
      summary: Check a user's TOU status
      description: "Check whether or not a User has accepted Quovo\u2019s terms of
        use."
      operationId: UsersTermsOfUseByUserIdGet
      x-api-path-slug: usersuser-idterms-of-use-get
      parameters:
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Check
      - Users
      - TOU
      - Status
    put:
      summary: Update a user's TOU status
      description: "Update whether or not a User has accepted Quovo\u2019s terms of
        use."
      operationId: UsersTermsOfUseByUserIdPut
      x-api-path-slug: usersuser-idterms-of-use-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - TOU
      - Status
  /tokens:
    get:
      summary: Get all active access tokens
      description: Retrieves all of your current Access Tokens.
      operationId: TokensGet
      x-api-path-slug: tokens-get
      responses:
        200:
          description: OK
      tags:
      - Active
      - Access
      - Tokens
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