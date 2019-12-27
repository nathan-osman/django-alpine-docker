FROM alpine:latest
LABEL maintainer="Nathan Osman <nathan@quickmediasolutions.com>"

# Install Python 3 and Django
RUN \
    apk add --no-cache \
        uwsgi-http \
        uwsgi-python && \
    pip3 install --no-cache-dir Django
