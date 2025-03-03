- OAuth scopes  - access levels, providing transparency to client on what they are permitting the client to do during the authorization process.
- OAuth flows - 
    - Authorization code flow 
    client gets authorization code through the login process and grants consent; Then client use the authorization code, client id and client secret to get access token and refresh token.
    - Implicit flow ???
    - Resource owner password credentials flow 
    - Client credentials flow ???


https://frontegg.com/blog/oauth

Case Study 

- Slack Integration 
    - Bot Token uses OAuth flow, the authorization process happens when user installs the app, and grants access to the bot token. Bot token is used to access the Slack API on behalf of the user. Bot token is shared across all users in the same workspace.

    - Bot token: represents what the Bot user can do on slack.
    - User token: used to perform actions on slack on behalf of the user.

    - For each workspace, there will be a bot token and potentially a user token requested. If slack app is built to be installed on different workspaces, then we will need a store the manage the tokens, that can be firebase. 
    https://tools.slack.dev/bolt-js/concepts/authenticating-oauth
    OAuth flow for slack app is still not natural ???

- QuickBooks Integration


