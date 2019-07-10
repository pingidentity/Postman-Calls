# PingAccess Admin API Postman collection

Postman Collection demonstrating how to use the [PingAccess](https://support.pingidentity.com/s/document-item?bundleId=pingaccess-52&topicId=overview%2Fpa_c_PingAccess_Overview.html) Admin REST API.  Note, this collection was built against PingAccess v5.2.3.  More information about the PingAccess Admin API can be found on [support.pingidentity.com](https://support.pingidentity.com/s/document-item?bundleId=pingaccess-52&topicId=reference/api/pa_c_Administrative_API_Endpoints.html).

## Installation

To use the latest published version, click the following button to import the PingAccess Admin API as a collection:

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/d671fbbcc3fe9ccdf36a)

You can also download the collection file from this repo, then import directly into Postman.

### Prerequisites

- *Postman* The collection is for use by the Postman app. Postman is a utility that allows you to quickly test and use REST APIs. More information can be found at [getpostman.com](https://www.getpostman.com/).

## Usage

The collection is arranged in folders according to the Admin API endpoints.

All requests require the host of the PingAccess Admin node, Admin credentials, and the Admin API version.  The collection requests have placeholder environment variables called `host`, `un`, `pw`, and `v`, respectively, for these values.
You can setup these values in your [Postman environment](https://www.getpostman.com/docs/v6/postman/environments_and_globals/manage_environments).  There is also an environment file that can be downloaded from this repo, and imported directory into Postman for connivence.


More information on managing Postman environments and variables can be found [here](https://www.getpostman.com/docs/v6/postman/environments_and_globals/variables).

|Variable  |Default value               |Set in         |May override in  |Example|
|----------|----------------------------|---------------|-----------------|-------|
|`host`    |`localhost`                 |Environment    |Environment      |`localhost`|
|`un`      |`Administrator`             |Environment    |Environment      |`Administrator`|
|`pw`      |`2Access`                   |Environment    |Environment      |`2Access`|
|`v`       |`v3`                        |Environment    |Environment      |`v3`  |

### Change Log

[See ChangeLog here](CHANGELOG.md)

## See Also

[Ping Identity APIs](https://www.pingidentity.com/content/developer/en/explore.html)

[Postman API development tool](https://www.getpostman.com/)
