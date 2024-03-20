FROM nathanosman/django-alpine:psycopg2
LABEL maintainer="Nathan Osman <nathan@quickmediasolutions.com>"

# Install the required packages for building libsass; then remove them
RUN \
    apk add --no-cache \
        build-base \
        libstdc++ \
        python3-dev && \
    pip install --no-cache-dir --break-system-packages django-libsass django_compressor && \
    apk del \
        build-base \
        python3-dev
