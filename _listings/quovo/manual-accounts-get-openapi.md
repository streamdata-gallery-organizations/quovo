---
swagger: "2.0"
x-collection-name: Quovo
x-complete: 0
info:
  title: Quovo Get all manual accounts
  description: Retrieves all Manual Accounts across all Users.
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
    post:
      summary: Create a new access token
      description: Creates and returns a new Access Token.
      operationId: TokensPost4
      x-api-path-slug: tokens-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - New
      - Access
      - Token
    delete:
      summary: Delete an existing access token
      description: Deletes an Access Token.
      operationId: TokensDelete
      x-api-path-slug: tokens-delete
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Existing
      - Access
      - Token
  /connections/{connection_id}:
    get:
      summary: Get a single connection
      description: Provides information on a specific connection.
      operationId: ConnectionsByConnectionIdGet
      x-api-path-slug: connectionsconnection-id-get
      parameters:
      - in: path
        name: connection_id
      responses:
        200:
          description: OK
      tags:
      - Single
      - Connection
    put:
      summary: Modify a connection
      description: Modifies an existing connection.
      operationId: ConnectionsByConnectionIdPut
      x-api-path-slug: connectionsconnection-id-put
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
      - Modify
      - Connection
    delete:
      summary: Delete a connection
      description: Deletes an existing Quovo connection.
      operationId: ConnectionsByConnectionIdDelete
      x-api-path-slug: connectionsconnection-id-delete
      parameters:
      - in: path
        name: connection_id
      responses:
        200:
          description: OK
      tags:
      - Connection
  /users/{user_id}:
    get:
      summary: Get a single user
      description: Provides information on a single User.
      operationId: UsersByUserIdGet
      x-api-path-slug: usersuser-id-get
      parameters:
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Single
      - User
    put:
      summary: Modify a user
      description: Modifies an existing User.
      operationId: UsersByUserIdPut
      x-api-path-slug: usersuser-id-put
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
      - Modify
      - User
    delete:
      summary: Delete a User
      description: Deletes a Quovo User.
      operationId: UsersByUserIdDelete
      x-api-path-slug: usersuser-id-delete
      parameters:
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
  /users:
    get:
      summary: Get all users
      description: Fetches all of your Users.
      operationId: UsersGet
      x-api-path-slug: users-get
      responses:
        200:
          description: OK
      tags:
      - Users
    post:
      summary: Create a new Quovo User
      description: |-
        Creates a new Quovo User.

        Users are owners of Accounts, Portfolios, and any related financial data such as Positions and History.

        If you have a Postman Environment set up, the previous request should have set your Access Token automatically. If not, be sure that your Access Token is included in the current request:

        1. Click on the "Headers" tab.
        2. Enter `Authorization` as the header field.
        3. Enter `Bearer token` as the header value, where `token` should be replaced with your actual Access Token.

        After sending the request, the Environment variable `user_id` will be automatically set to the newly created User's id.
      operationId: UsersPost4
      x-api-path-slug: users-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - New
      - Quovo
      - User
  /connections/{connection_id}/transactions:
    get:
      summary: Get a connection's transactions
      description: Provides information on a connection's historical transactions.
      operationId: ConnectionsTransactionsByConnectionIdGet
      x-api-path-slug: connectionsconnection-idtransactions-get
      parameters:
      - in: path
        name: connection_id
      responses:
        200:
          description: OK
      tags:
      - Connections
      - Transactions
  /connections:
    get:
      summary: Get  all connections
      description: Retrieves all connections across all users.
      operationId: ConnectionsGet
      x-api-path-slug: connections-get
      responses:
        200:
          description: OK
      tags:
      - Connections
  /institutions:
    get:
      summary: Get all institutions
      description: Provides information on all of Quovo's supported institutions.
      operationId: InstitutionsGet
      x-api-path-slug: institutions-get
      responses:
        200:
          description: OK
      tags:
      - Institutions
  /connections/{connection_id}/accounts:
    get:
      summary: Fetch the Connection's Accounts
      description: |-
        Fetches all of the accounts belonging to the connection. These are automatically created by Quovo after an initial sync.

        If you have a Postman Environment set up, this request will automatically set the variable `account_id` to the id of the first account returned.
      operationId: ConnectionsAccountsByConnectionIdGet4
      x-api-path-slug: connectionsconnection-idaccounts-get
      parameters:
      - in: path
        name: connection_id
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - Connections
      - Accounts
  /users/{user_id}/connections:
    get:
      summary: Get a user's connections
      description: Returns all of a user's connections.
      operationId: UsersConnectionsByUserIdGet
      x-api-path-slug: usersuser-idconnections-get
      parameters:
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Connections
    post:
      summary: Create a Connection
      description: Creates a new Quovo Connection.
      operationId: UsersConnectionsByUserIdPost4
      x-api-path-slug: usersuser-idconnections-post
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
      - Connection
  /me:
    get:
      summary: Get info about your API user
      description: Fetch information about your Quovo API user.
      operationId: MeGet
      x-api-path-slug: me-get
      responses:
        200:
          description: OK
      tags:
      - Info
      - About
      - Your
      - User
    put:
      summary: Update your password
      description: "Update your API password. All future requests to /v3/tokens must
        use the new password to properly authenticate.\r\n\r\nNew API passwords have
        several requirements:\r\n\r\n* Must be at least 6 characters long\r\n* Must
        contain a letter, a number, and a special character\r\n* Must not contain
        or be similar to your registered email or Quovo API username"
      operationId: MePut
      x-api-path-slug: me-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Your
      - Password
  /users/{user_id}/holdings:
    get:
      summary: Get a user's holdings
      description: Fetches all holdings for a specific user.
      operationId: UsersHoldingsByUserIdGet
      x-api-path-slug: usersuser-idholdings-get
      parameters:
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Holdings
  /users/{user_id}/institution_requests:
    post:
      summary: Request a new institution
      description: Requests a new financial institution for Quovo to retrieve data
        from.
      operationId: UsersInstitutionRequestsByUserIdPost
      x-api-path-slug: usersuser-idinstitution-requests-post
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
      - Request
      - New
      - Institution
  /webhooks:
    get:
      summary: Get all registered webhooks
      description: "Retrieve your registered webhooks. \n\nNote: secret is intentionally
        omitted from all GET requests. It is only returned after being updated or
        after a new webhook is created."
      operationId: WebhooksGet
      x-api-path-slug: webhooks-get
      responses:
        200:
          description: OK
      tags:
      - Registered
      - Webhooks
    put:
      summary: Update an existing webhook
      description: Used to update an existing webhook.
      operationId: WebhooksPut
      x-api-path-slug: webhooks-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Existing
      - Webhook
    post:
      summary: Register a new webhook
      description: Used to register new webhooks.
      operationId: WebhooksPost
      x-api-path-slug: webhooks-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Register
      - New
      - Webhook
    delete:
      summary: Delete a webhook
      description: Deletes an existing webhook.
      operationId: WebhooksDelete
      x-api-path-slug: webhooks-delete
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Webhook
  /connections/{connection_id}/challenges:
    get:
      summary: Get challenges for a connection
      description: Retrieves any Challenges associated with a connection.
      operationId: ConnectionsChallengesByConnectionIdGet
      x-api-path-slug: connectionsconnection-idchallenges-get
      parameters:
      - in: path
        name: connection_id
      responses:
        200:
          description: OK
      tags:
      - Challengesa
      - Connection
    put:
      summary: Answer MFA challenges
      description: Answer available MFA Challenges for a connection.
      operationId: ConnectionsChallengesByConnectionIdPut
      x-api-path-slug: connectionsconnection-idchallenges-put
      parameters:
      - in: path
        name: connection_id
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Answer
      - MFA
      - Challenges
  /holdings:
    get:
      summary: Get all holdings
      description: Fetches all holdings across all accounts and connections.
      operationId: HoldingsGet
      x-api-path-slug: holdings-get
      responses:
        200:
          description: OK
      tags:
      - Holdings
  /accounts/{account_id}/holdings:
    get:
      summary: Get an account's holdings
      description: Fetches all holdings for a specific account.
      operationId: AccountsHoldingsByAccountIdGet
      x-api-path-slug: accountsaccount-idholdings-get
      parameters:
      - in: path
        name: account_id
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Holdings
  /manual_accounts/{manual_account_id}:
    get:
      summary: Get a single manual account
      description: Returns a single Manual Account.
      operationId: ManualAccountsByManualAccountIdGet
      x-api-path-slug: manual-accountsmanual-account-id-get
      parameters:
      - in: path
        name: manual_account_id
      responses:
        200:
          description: OK
      tags:
      - Single
      - Manual
      - Account
    put:
      summary: Update a manual account
      description: Modifies a Manual Account.
      operationId: ManualAccountsByManualAccountIdPut
      x-api-path-slug: manual-accountsmanual-account-id-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: manual_account_id
      responses:
        200:
          description: OK
      tags:
      - Manual
      - Account
    delete:
      summary: Delete a manual account
      description: Deletes a Manual Account.
      operationId: ManualAccountsByManualAccountIdDelete
      x-api-path-slug: manual-accountsmanual-account-id-delete
      parameters:
      - in: path
        name: manual_account_id
      responses:
        200:
          description: OK
      tags:
      - Manual
      - Account
  /accounts/{account_id}/extras:
    get:
      summary: Fetch an Account's Extras Information
      description: Retrieves an Account's Extras Information.
      operationId: AccountsExtrasByAccountIdGet
      x-api-path-slug: accountsaccount-idextras-get
      parameters:
      - in: path
        name: account_id
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - Accounts
      - Extras
      - Information
  /manual_accounts/{manual_account_id}/manual_holdings:
    get:
      summary: Get a manual account's holdings
      description: Fetches all of the Portfolio's Manual Assets.
      operationId: ManualAccountsManualHoldingsByManualAccountIdGet
      x-api-path-slug: manual-accountsmanual-account-idmanual-holdings-get
      parameters:
      - in: path
        name: manual_account_id
      responses:
        200:
          description: OK
      tags:
      - Manual
      - Accounts
      - Holdings
    put:
      summary: Update a manual holding
      description: Updates an existing Manual Asset for the given Manual Portfolio.
      operationId: ManualAccountsManualHoldingsByManualAccountIdPut
      x-api-path-slug: manual-accountsmanual-account-idmanual-holdings-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: manual_account_id
      responses:
        200:
          description: OK
      tags:
      - Manual
      - Holding
    post:
      summary: Create a manual holding
      description: Creates a new Manual Asset for the given Manual Portfolio.
      operationId: ManualAccountsManualHoldingsByManualAccountIdPost
      x-api-path-slug: manual-accountsmanual-account-idmanual-holdings-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: manual_account_id
      responses:
        200:
          description: OK
      tags:
      - Manual
      - Holding
    delete:
      summary: Delete a manual holding
      description: Deletes an existing Manual Asset for the given Manual Portfolio.
      operationId: ManualAccountsManualHoldingsByManualAccountIdDelete
      x-api-path-slug: manual-accountsmanual-account-idmanual-holdings-delete
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: manual_account_id
      responses:
        200:
          description: OK
      tags:
      - Manual
      - Holding
  /users/{user_id}/manual_accounts:
    get:
      summary: Get a user's manual accounts
      description: Returns all Manual Portfolios of a given User.
      operationId: UsersManualAccountsByUserIdGet
      x-api-path-slug: usersuser-idmanual-accounts-get
      parameters:
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Manual
      - Accounts
    post:
      summary: Create a manual account
      description: Creates a Manual Account.
      operationId: UsersManualAccountsByUserIdPost
      x-api-path-slug: usersuser-idmanual-accounts-post
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
      - Manual
      - Account
  /accounts/{account_id}/transactions:
    get:
      summary: Get an account's transactions
      description: Provides information on an account's historical transactions.
      operationId: AccountsTransactionsByAccountIdGet
      x-api-path-slug: accountsaccount-idtransactions-get
      parameters:
      - in: path
        name: account_id
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Transactions
  /connections/{connection_id}/manual_holdings:
    get:
      summary: Get a connection's manual holdings
      description: Fetches all Manual Assets for an Account.
      operationId: ConnectionsManualHoldingsByConnectionIdGet
      x-api-path-slug: connectionsconnection-idmanual-holdings-get
      parameters:
      - in: path
        name: connection_id
      responses:
        200:
          description: OK
      tags:
      - Connections
      - Manual
      - Holdings
  /users/{user_id}/transactions:
    get:
      summary: Get a user's transactions
      description: Provides historical transactions for a specific user.
      operationId: UsersTransactionsByUserIdGet
      x-api-path-slug: usersuser-idtransactions-get
      parameters:
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Transactions
  /manual_accounts:
    get:
      summary: Get all manual accounts
      description: Retrieves all Manual Accounts across all Users.
      operationId: ManualAccountsGet
      x-api-path-slug: manual-accounts-get
      responses:
        200:
          description: OK
      tags:
      - Manual
      - Accounts
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