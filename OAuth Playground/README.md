# PingFed-OAuth-Playground

This is a Postman collection that demonstrates PingFederate as an Oauth \ OIDC AS without using any UI.

It assumes that an install of the PingFed OAuth playground has been performed, with seperate OAuth clients for each flow.
https://www.pingidentity.com/en/resources/downloads/pingfederate.html

Update: 11/25/18
* Added the following flows:
   * SAML Bearer
   * JWT Bearer
   * Device Flow (PF 9.2+)
* Added examples using x-www-form-urlencoded body for call parameters
* Organized calls a little better
* Indicated PF versions for more recent support
* Included Postman Environment file

Update: 11/26/18
* Added Scope parameter \ field to all requests
* Added Client Credential with client_assertion JWT flow
