# Authorisation

Our API is secured through a token based authentication.
The token, provided by SmartEDi-TORS, has to be present with each request, as a header.

SmartED-i requires the token to be included in all API requests to the server in a header that looks like the following:

`token: SmartEDi-token`

<aside class="notice">
You must replace <code>SmartEDi-token</code> with your personal token.
</aside>

User must also be authenticated (see sessions/authenticate).