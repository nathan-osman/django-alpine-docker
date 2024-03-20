FROM nathanosman/django-alpine:base
LABEL maintainer="Nathan Osman <nathan@quickmediasolutions.com>"

# Install the required packages for building psycopg2; then remove them
RUN \
    apk add --no-cache \
        build-base \
        libpq \
        postgresql-dev \
        python3-dev && \
    pip install --no-cache-dir --break-system-packages psycopg2 && \
    apk del \
        build-base \
        postgresql-dev \
        python3-dev
