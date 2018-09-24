# Postman-Calls

This repository is a collection of Postman calls that can be made against Ping Identity products.

## OAuth-Playground
Full set of calls made to demonstrate various OAuth flows without needing an application to perform them.

Calls marked with (Browser) are intended to be pasted into a Browser to make the initial call for an Authorization Code or an Implicit access_token

The redirect_uri can be any URL that will accept the response from PingFederate. In these calls, it's a simple webpage that will display the response parameters
