## Bearer Authorization
1-Write the following steps in the correct order:

- 1. Register your application to get a client_id and client_secret
- 2. Make a request to a third-party API endpoint
- 3. Redirect to a third-party authentication endpoint
- 4. Receive authorization code
- 5. Ask the client if they want to sign in via a third party
- 6. Make a request to the access token endpoint

2-What can you do with an authorization code?
process of determining if the user has permission to perform a given operation.

3-What can you do with an access token?
We store this token on the client and send it to the server every time we need to call an API endpoint that is only accessible to authenticated users.

4-What’s a benefit of using OAuth instead of your own basic authentication?
We use them to identify users. It’s similar to a passport or driver’s license. It includes a few public properties about a user in its payload. These properties cannot be tampered because doing so requires re-generating the digital signature.

## Terms:
-Client ID: a public identifier for apps

-Client Secret: secret known only to the application and the authorization server

-Authentication endpoint: where the user is sent to input credentials to become authorized
Access Token Endpoint: where apps make a request to get an access token for a user

-API Endpoint: can include a URL of a server or service, each endpoint is the location from which APIs can access the resources they need to carry out their function

-Authorization Code: temporary code that the client will exchange for an access token
Access Token: the thing that applications use to make API requests on behalf of a user
### (JWT) 
JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.