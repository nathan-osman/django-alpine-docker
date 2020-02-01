## django-alpine-docker

[![Build Status](https://ci.quickmediasolutions.com/buildStatus/icon?job=django-alpine-docker)](https://ci.quickmediasolutions.com/job/django-alpine-docker/)
[![MIT License](http://img.shields.io/badge/license-MIT-9370d8.svg?style=flat)](http://opensource.org/licenses/MIT)

This repository builds three Docker images:

#### nathanosman/docker-alpine:base

This image provides the bare minimum necessary for running a Django application. This currently includes uWSGI and the Django Python package.

#### nathanosman/docker-alpine:psycopg2

This image provides everything in the base image as well as the psycopg2 Python package, enabling support for PostgreSQL database connections.

#### nathanosman/docker-alpine:compressor

This image provides everything in the psycopg2 image as well as django-compressor and the libsass library.

#### nathanosman/docker-alpine:pillow

This image provides everything in the compressor image as well as the Pillow Python package, enabling image reading / writing / editing.
