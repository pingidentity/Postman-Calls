# Postman-Calls

This repository is a collection of Postman calls that can be made against Ping Identity products.

## OAuth-Playground
Full set of calls made to demonstrate various OAuth flows without needing an application to perform them.

Calls marked with (Browser) are intended to be pasted into a Browser to make the initial call for an Authorization Code or an Implicit access_token

The redirect_uri can be any URL that will accept the response from PingFederate. In these calls, it's a simple webpage (https://apps.cpricedomain.net/OAuthDecode) that will display the response parameters

OAuth Playground clients are prefixed with "play_" - i.e. play_ac_client - if you change these, also modify the Authorization Basic header contents to match your client settings.
