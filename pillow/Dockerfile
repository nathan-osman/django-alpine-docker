FROM nathanosman/django-alpine:psycopg2
LABEL maintainer="Nathan Osman <nathan@quickmediasolutions.com>"

# Install the required packages for building Pillow; then remove them
#  (Pillow is built with support for JPEG and PNG)
RUN \
    apk add --no-cache \
        build-base \
        jpeg-dev \
        zlib-dev && \
    pip3 install --no-cache-dir Pillow && \
    apk del \
        build-base \
        jpeg-dev \
        zlib-dev
