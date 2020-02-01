FROM nathanosman/django-alpine:psycopg2
LABEL maintainer="Nathan Osman <nathan@quickmediasolutions.com>"

# Install the required packages for building libsass; then remove them
RUN \
    apk add --no-cache \
        build-base \
        libstdc++ \
        python3-dev && \
    pip3 install --no-cache-dir django-compressor && \
    apk del \
        build-base \
        python3-dev
