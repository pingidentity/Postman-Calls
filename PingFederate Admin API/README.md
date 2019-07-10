# PingFederate Admin API Postman collection

Postman Collection demonstrating how to use the [PingFederate](https://support.pingidentity.com/s/document-item?bundleId=pingfederate-93&topicId=gettingStartedGuide%2FgettingStarted.html) Admin REST API.  Note, this collection was built against PingFederate v9.3.0.  More information about the PingFederate Admin API can be found on [support.pingidentity.com](https://support.pingidentity.com/s/document-item?bundleId=pingfederate-93&topicId=adminGuide%2FpingFederateAdministrativeApi.html).

## Installation

To use the latest published version, click the following button to import the PingFederate Admin API as a collection:

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/6347ba9962c564395251)

You can also download the collection file from this repo, then import directly into Postman.

### Prerequisites

- *Postman* The collection is for use by the Postman app. Postman is a utility that allows you to quickly test and use REST APIs. More information can be found at [getpostman.com](https://www.getpostman.com/).

## Usage

The collection is arranged in folders according to the Admin API endpoints.

All requests require the host of the PingFederate Admin node, and the Admin credentials.  The collection requests have placeholder environment variables called `host`, `un`, and `pw`, respectively, for these values.
You can setup these values in your [Postman environment](https://www.getpostman.com/docs/v6/postman/environments_and_globals/manage_environments).  There is also an environment file that can be downloaded from this repo, and imported directory into Postman for convenience.


More information on managing Postman environments and variables can be found [here](https://www.getpostman.com/docs/v6/postman/environments_and_globals/variables).

|Variable  |Default value               |Set in         |May override in  |Example|
|----------|----------------------------|---------------|-----------------|-------|
|`host`    |`localhost`                 |Environment    |Environment      |`localhost`|
|`un`      |`Administrator`             |Environment    |Environment      |`Administrator`|
|`pw`      |`2Federate`                 |Environment    |Environment      |`2Federate`|

### Change Log

[See ChangeLog here](CHANGELOG.md)

## See Also

[Ping Identity APIs](https://www.pingidentity.com/content/developer/en/explore.html)

[Postman API development tool](https://www.getpostman.com/)
