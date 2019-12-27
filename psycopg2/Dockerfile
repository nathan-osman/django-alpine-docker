FROM nathanosman/django-alpine:base
LABEL maintainer="Nathan Osman <nathan@quickmediasolutions.com>"

# Install the required packages for building psycopg2; then remove them
RUN \
    apk add --no-cache \
        build-base \
        postgresql-dev \
        python3-dev && \
    pip3 install --no-cache-dir psycopg2 && \
    apk del \
        build-base \
        postgresql-dev \
        python3-dev
