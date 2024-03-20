FROM alpine:latest
LABEL maintainer="Nathan Osman <nathan@quickmediasolutions.com>"

# Install Python 3 and Django
RUN \
    apk add --no-cache \
        uwsgi-http \
        uwsgi-python \
        py3-pip && \
    pip install --no-cache-dir --break-system-packages Django
