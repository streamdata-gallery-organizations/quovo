---
name: Quovo
x-slug: quovo
description: Quovo&rsquo;s API provides methods for retrieving data from financial
  institutions on behalf of clients, advisors, and other users. This documentation
  includes detailed explanations of API endpoints and common data definitions. Please
  note that this documentation does not list all API endpoints. Additionally, you
  may not have access to all of the listed endpoints depending on the services you&rsquo;ve
  purchased from Quovo.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
x-kinRank: "7"
x-alexaRank: "391003"
tags: Quovo
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/apis.md
specificationVersion: "0.14"
apis:
- name: Quovo API v3 - Get a connection's sync progress
  x-api-slug: connectionsconnection-idsync-get
  description: Check the ongoing Sync progress of an Account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/connectionsconnection-idsync-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/connectionsconnection-idsync-get-openapi.md
- name: Quovo API v3 - Check a user's TOU status
  x-api-slug: usersuser-idterms-of-use-get
  description: "Check whether or not a User has accepted Quovo\u2019s terms of use."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/usersuser-idterms-of-use-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/usersuser-idterms-of-use-get-openapi.md
- name: Quovo API v3 - Get all active access tokens
  x-api-slug: tokens-get
  description: Retrieves all of your current Access Tokens.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/tokens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/tokens-get-openapi.md
- name: Quovo API v3 - Get a single user
  x-api-slug: usersuser-id-get
  description: Provides information on a single User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/usersuser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/usersuser-id-get-openapi.md
- name: Quovo API v3 - Get a connection's transactions
  x-api-slug: connectionsconnection-idtransactions-get
  description: Provides information on a connection's historical transactions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/connectionsconnection-idtransactions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/connectionsconnection-idtransactions-get-openapi.md
- name: Quovo API v3 - Get  all connections
  x-api-slug: connections-get
  description: Retrieves all connections across all users.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/connections-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/connections-get-openapi.md
- name: Quovo API v3 - Get all institutions
  x-api-slug: institutions-get
  description: Provides information on all of Quovo's supported institutions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/institutions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/institutions-get-openapi.md
- name: Quovo API v3 - Fetch the Connection's Accounts
  x-api-slug: connectionsconnection-idaccounts-get
  description: |-
    Fetches all of the accounts belonging to the connection. These are automatically created by Quovo after an initial sync.

    If you have a Postman Environment set up, this request will automatically set the variable `account_id` to the id of the first account returned.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/connectionsconnection-idaccounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/connectionsconnection-idaccounts-get-openapi.md
- name: Quovo API v3 - Get a user's connections
  x-api-slug: usersuser-idconnections-get
  description: Returns all of a user's connections.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/usersuser-idconnections-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/usersuser-idconnections-get-openapi.md
- name: Quovo API v3 - Get info about your API user
  x-api-slug: me-get
  description: Fetch information about your Quovo API user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/me-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/me-get-openapi.md
- name: Quovo API v3 - Answer MFA challenges
  x-api-slug: connectionsconnection-idchallenges-put
  description: Answer available MFA Challenges for a connection.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/connectionsconnection-idchallenges-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/connectionsconnection-idchallenges-put-openapi.md
- name: Quovo API v3 - Get an account's holdings
  x-api-slug: accountsaccount-idholdings-get
  description: Fetches all holdings for a specific account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/accountsaccount-idholdings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/accountsaccount-idholdings-get-openapi.md
- name: Quovo API v3 - Get a single manual account
  x-api-slug: manual-accountsmanual-account-id-get
  description: Returns a single Manual Account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/manual-accountsmanual-account-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/manual-accountsmanual-account-id-get-openapi.md
- name: Quovo API v3 - Fetch an Account's Extras Information
  x-api-slug: accountsaccount-idextras-get
  description: Retrieves an Account's Extras Information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/accountsaccount-idextras-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/accountsaccount-idextras-get-openapi.md
- name: Quovo API v3 - Get a manual account's holdings
  x-api-slug: manual-accountsmanual-account-idmanual-holdings-get
  description: Fetches all of the Portfolio's Manual Assets.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/manual-accountsmanual-account-idmanual-holdings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/manual-accountsmanual-account-idmanual-holdings-get-openapi.md
- name: Quovo API v3 - Get a user's manual accounts
  x-api-slug: usersuser-idmanual-accounts-get
  description: Returns all Manual Portfolios of a given User.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/usersuser-idmanual-accounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/usersuser-idmanual-accounts-get-openapi.md
- name: Quovo API v3 - Get an account's transactions
  x-api-slug: accountsaccount-idtransactions-get
  description: Provides information on an account's historical transactions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/accountsaccount-idtransactions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/accountsaccount-idtransactions-get-openapi.md
- name: Quovo API v3 - Get a connection's manual holdings
  x-api-slug: connectionsconnection-idmanual-holdings-get
  description: Fetches all Manual Assets for an Account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/connectionsconnection-idmanual-holdings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/connectionsconnection-idmanual-holdings-get-openapi.md
- name: Quovo API v3 - Get all manual accounts
  x-api-slug: manual-accounts-get
  description: Retrieves all Manual Accounts across all Users.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/manual-accounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/manual-accounts-get-openapi.md
- name: Quovo API v3 - Get all accounts
  x-api-slug: accounts-get
  description: Fetches all Accounts accross all Users.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/accounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/accounts-get-openapi.md
- name: Quovo API v3 - Get a connection's holdings
  x-api-slug: connectionsconnection-idholdings-get
  description: Fetches all holdings for a specific connection.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/connectionsconnection-idholdings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/connectionsconnection-idholdings-get-openapi.md
- name: Quovo API v3 - Get a single transaction
  x-api-slug: transactionstransaction-id-get
  description: Provides information on a single historical transaction.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/transactionstransaction-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/transactionstransaction-id-get-openapi.md
- name: Quovo API v3 - Get a user's accounts
  x-api-slug: usersuser-idaccounts-get
  description: Fetches all Accounts for a specific user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28293-quovo.jpg
  humanURL: http://quovo.com
  baseURL: https://example.com//
  tags: SaaS, Technology, Enterprise, Financial Services, Financial, Market Data,
    Profiles, General Data, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/usersuser-idaccounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/quovo/master/_listings/quovo/usersuser-idaccounts-get-openapi.md
x-common:
- type: x-blog-rss
  url: https://www.quovo.com/fintech-blog/feed/
- type: x-postman-collection
  url: https://www.getpostman.com/collections/82cf673bb22d4f8b8881
- type: x-website
  url: http://quovo.com
- type: x-api-gallery
  url: http://quandl.api.gallery.streamdata.io
- type: x-api-stack
  url: http://quovo.stack.network
- type: x-authentication
  url: https://api.quovo.com/docs/v3/#authentication
- type: x-blog
  url: https://www.quovo.com/fintech-blog/
- type: x-crunchbase
  url: https://crunchbase.com/organization/quovo
- type: x-developer
  url: https://api.quovo.com/docs/v3/
- type: x-email
  url: audit@quovo.com
- type: x-email
  url: info@quovo.com
- type: x-email
  url: copyright@quovo.com
- type: x-email
  url: support@quovo.com
- type: x-github
  url: https://github.com/quovo
- type: x-twitter
  url: https://twitter.com/quovo
- type: x-webhook
  url: https://api.quovo.com/docs/v3/#webhooks
- type: x-website
  url: https://www.quovo.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---