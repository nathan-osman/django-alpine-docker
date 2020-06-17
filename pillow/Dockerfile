FROM nathanosman/django-alpine:compressor
LABEL maintainer="Nathan Osman <nathan@quickmediasolutions.com>"

# Install the required packages for building Pillow; then remove them
#  (Pillow is built with support for JPEG and PNG)
RUN \
    apk add --no-cache \
        build-base \
        jpeg \
        jpeg-dev \
        python3-dev \
        zlib-dev && \
    pip install --no-cache-dir Pillow && \
    apk del \
        build-base \
        jpeg-dev \
        python3-dev \
        zlib-dev
