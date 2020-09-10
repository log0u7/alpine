# Alpine Docker Container Image

[![Build Status](https://travis-ci.org/log0u7/alpine.svg?branch=master)](https://travis-ci.org/log0u7/alpine)
[![Docker Pulls](https://img.shields.io/docker/pulls/log0u7/alpine.svg)](https://hub.docker.com/r/log0u7/alpine)
[![Docker Stars](https://img.shields.io/docker/stars/log0u7/alpine.svg)](https://hub.docker.com/r/log0u7/alpine)
[![Docker Layers](https://images.microbadger.com/badges/image/log0u7/alpine.svg)](https://microbadger.com/images/log0u7/alpine)

This is a basic alpine image used in log0u7's docker images
This use [wodby gotpl](https://github.com/wodby/gotpl) fixed release for templating (will be moved soon for ansible)

## Docker Images

❗For better reliability only use images with stability tags (`log0u7/alpine:3-X.X.X`) which correspond to [git tags](https://github.com/log0u7/alpine/releases).

About images:

* All images based on Alpine Linux
* Base image: [alpine](https://hub.docker.com/r/_/alpine)
* [Travis CI builds](https://travis-ci.org/log0u7/alpine)
* [Docker Hub](https://hub.docker.com/r/log0u7/alpine)

[_(Dockerfile)_]: https://github.com/log0u7/alpine/tree/master/Dockerfile

Supported tags and respective `Dockerfile` links:

* `3.12`, `3`, `latest` [_(Dockerfile)_]
* `3.11` [_(Dockerfile)_]
* `3.10` [_(Dockerfile)_]
* `3.9` [_(Dockerfile)_]
* `3.8` [_(Dockerfile)_]
* `3.12-dev`, `3-dev`, `dev` [_(Dockerfile)_]

## Scripts

This image contains the following helper scripts:

* `compare_semver` - compares two semantic versions
* `exec_init_scripts` - execute all `.sh` scripts from `/docker-entrypoint-init.d/`. Useful to have in every docker image
* `gen_ssh_keys` - generates SSH keys
* `gen_ssl_certs` - generate SSL certificates
* `get_archive` - copies (or downloads) and unpacks an archive
* `gpg_verify` - verify GPG signature from a list of key servers
* `gpg_decrypt` - decrypt an artifact that contains GPG signature
* `wait_for` - executes a command with for N times with N timeout until it return 0

See [`test.sh`](https://github.com/log0u7/alpine/blob/master/test.sh) for examples.
