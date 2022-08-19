# Building the ActiveMQ Artemis Docker Image

Depending on your platform the build process may differ slightly. Support for as many build platforms as possible is provided in a best effort basis.

If you consistently can reproduce a test failure, please search for it in the [issue tracker](https://github.com/kahootali/activemq-artemis-docker/issues) or file a new issue.

## Prerequisites

To build the ActiveMQ Artemis Docker Image the following tools are necessary:

- Docker

## Supported Platforms

Only UN*X based operating systems are supported currently for building this image.

## Building the image

You can build the image for whichever platform you want e.g. Debian or Alpine. Both Dockerfiles are present under `src` folder. Also you can pass in the `ACTIVEMQ_ARTEMIS_VERSION` as builder arg to whichever version you want. e.g

```bash
cd src/
docker build --builder-arg ACTIVEMQ_ARTEMIS_VERSION=2.17.0 -t activemq-artemis-docker .

```
