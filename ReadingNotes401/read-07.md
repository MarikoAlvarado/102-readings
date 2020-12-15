# Bearer Authorization

**Write the following steps in the correct order:**

1. Register your application to get a client_id and client_secret

2. Receive authorization code

3. Make a request to a third-party API endpoint

4. Ask the client if they want to sign in via a third party

5. Receive access token

6. Make a request to the access token endpoint

7. Redirect to a third party authentication endpoint

^^^^^???????^^^^^

**What can you do with an authorization code?**

You can use it to give the user a preview of what information they are requesting so that they can approve or deny the request. If they approve it they will exchange for an access token

**What can you do with an access token?**

You can use it as a more secure way of passing the authorization code for a user so a hacker can't access it.

^^^^^^ [source](https://www.oauth.com/oauth2-servers/server-side-apps/authorization-code/#:~:text=The%20authorization%20code%20is%20a,approve%20or%20deny%20the%20request.) ^^^^^^


**What’s a benefit of using OAuth instead of your own basic authentication?**

It's more secure because it uses encryption.

### Terms

**Client ID** - public identifier for applications that is unique for all clients a server handles

**Client Secret** - a server generated *random* secret only know by the app and auth server

^^ [source](https://www.oauth.com/oauth2-servers/client-registration/client-id-secret/) ^^

**Authentication Endpoint** - used to request access tokens or auth codes [source](https://identityserver.github.io/Documentation/docsv2/endpoints/authorization.html)

**Access Token Endpoint** - Requested endpoint that gives users an access token

**API Endpoint** - Where an api sends requests for data


**Authorization Code** - What the user approves/denies in return for an access token to an API endpoint


**Access Token** - unique to each user to have access to an API endpoint

### Skim

[Intro to JWT](https://jwt.io/introduction/)

[Are JWTs Secure?](https://stackoverflow.com/questions/27301557/if-you-can-decode-jwt-how-are-they-secure)

**bookmarked**

[npm jsonwebtoken docs](https://stackoverflow.com/questions/27301557/if-you-can-decode-jwt-how-are-they-secure)