# prh

[![CircleCI](https://circleci.com/gh/tmknom/prh.svg?style=svg)](https://circleci.com/gh/tmknom/prh)
[![Docker Build Status](https://img.shields.io/docker/cloud/build/tmknom/prh.svg)](https://hub.docker.com/r/tmknom/prh/builds/)
[![Docker Automated build](https://img.shields.io/docker/cloud/automated/tmknom/prh.svg)](https://hub.docker.com/r/tmknom/prh/)
[![MicroBadger Size](https://img.shields.io/microbadger/image-size/tmknom/prh.svg)](https://microbadger.com/images/tmknom/prh)
[![MicroBadger Layers](https://img.shields.io/microbadger/layers/tmknom/prh.svg)](https://microbadger.com/images/tmknom/prh)
[![License](https://img.shields.io/github/license/tmknom/prh.svg)](https://opensource.org/licenses/Apache-2.0)

A proofreading helper.

This is [prh](https://github.com/prh/prh) wrapper.

## Requirements

- [Docker](https://www.docker.com/)

## Usage

### Proofread markdown

```sh
docker run --rm -v "$PWD:/work" tmknom/prh --rules prh.yml **/*.md
```

### Help

```sh
docker run --rm -v "$PWD:/work" tmknom/prh
```

## Makefile targets

```text
build                          Build docker image
format                         Format code
help                           Show help
install                        Install requirements
lint                           Lint code
```

## Development

### Installation

```shell
git clone git@github.com:tmknom/prh.git
cd prh
make install
```

### Deployment

Automatically deployed by "[DockerHub Automated Build](https://docs.docker.com/docker-hub/builds/)" after merge.

### Deployment Pipeline

1. GitHub - Version Control System
   - <https://github.com/tmknom/prh>
2. CircleCI - Continuous Integration
   - <https://circleci.com/gh/tmknom/prh>
3. Docker Hub - Docker Registry
   - <https://hub.docker.com/r/tmknom/prh>
4. MicroBadger - Docker Inspection
   - <https://microbadger.com/images/tmknom/prh>

## License

Apache 2 Licensed. See LICENSE for full details.
