# PingID-Calls
After importing the pingid Postman Collection, all you need to do is set the Environment Variables (see below)
with information from your pingid.properties file, then on the "Pre-request Script" tab edit the "reqBody"
section to reflect the information or changes you wish to retrieve/make.

Reference the [PingID API docs](https://apidocs.pingidentity.com/pingid-api/guide/pingid-api/pid_c_PingIDapiOverview/) for more information on the "reqBody" content.

## Environment variables
1. org_alias (as appears in the PingID properties file)
2. token (as appears in the PingID properties file)
3. key (use_base64_key as appears in the PingID properties file)
4. idp_url (as appears in the PingID properties file)
5. version - the API version (see docs - usually 4.9)
