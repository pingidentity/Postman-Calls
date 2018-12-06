# Postman-Calls

This is a place to document calls to Ping APIs using Postman.

Some of the calls are individual, others may be to demonstrate a flow of transactions needed to perform a use case.

# OAuth Playground

This is Postman collection that demonstrates the OAuth \ OIDC flows without the UI of the PingFed OAuth Playground

# PingID SDK

These are examples of how to use the PingID SDK service to perform transactional MFA calls.

# Pre-Request script to generate a JWT

This call creates a signed JWT - it's used in the "OAuth Demo - Client Credentials with client_assertion (JWK)" call within the OAuth Playground collection, but can be used for anything.

The signature is handled by a sideloaded library - jsrsasign. The "Get jsrsasign library" call should be made to populate the code into a global variable that is invoked at the start of the pre-request script.

This script can work with both RSA and EC JWK objects - they can be generated from here:
https://mkjwk.org/

The Signing KeyPair should be stored in a Postman Environment

The script will use the JWK to define the Algorithm and KID that is used in the Signing
