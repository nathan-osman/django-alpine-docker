FROM alpine:latest
LABEL maintainer="Nathan Osman <nathan@quickmediasolutions.com>"

# Install Python 3 and Django
RUN \
    apk add --no-cache \
        python3 \
        uwsgi-http \
        uwsgi-python3 && \
    pip3 install --no-cache-dir Django
