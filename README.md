## django-alpine-docker

[![Build Status](https://ci.quickmediasolutions.com/buildStatus/icon?job=django-alpine-docker)](https://ci.quickmediasolutions.com/job/django-alpine-docker/)
[![MIT License](http://img.shields.io/badge/license-MIT-9370d8.svg?style=flat)](http://opensource.org/licenses/MIT)

This repository builds four Docker images:

#### nathanosman/docker-alpine:base

This image provides the bare minimum necessary for running a Django application. This currently includes [uWSGI](https://uwsgi-docs.readthedocs.io/en/latest/) and the [Django](https://www.djangoproject.com/) Python package.

#### nathanosman/docker-alpine:psycopg2

This image provides everything in the base image as well as the [psycopg2](https://pypi.org/project/psycopg2/) Python package, enabling support for PostgreSQL database connections.

#### nathanosman/docker-alpine:compressor

This image provides everything in the psycopg2 image as well as the [django-libsass](https://github.com/torchbox/django-libsass) and [django_compressor](https://github.com/django-compressor/django-compressor) Python packages, enabling full support for compiling SASS files and minifying scripts.

#### nathanosman/docker-alpine:pillow

This image provides everything in the compressor image as well as the [Pillow](https://pillow.readthedocs.io/en/stable/) Python package, enabling image reading / writing / editing.
