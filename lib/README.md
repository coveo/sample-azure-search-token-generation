# Coveo Search Token Generator

Node.js module that serves Coveo search tokens for Dynamics portal.

``` javascript
// Decodes the authentication token from portal to extract the payload.
const portalAuth: IDecodedPortalAuthTokenPayload = await portal.decodeAuthToken(req.headers.authorization);
// Gets a search token from Coveo for the user specified in the token.
const coveoSearchToken: string = await coveo.getSearchToken(portalAuth.email);
```