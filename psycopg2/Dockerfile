FROM nathanosman/django-alpine:base
LABEL maintainer="Nathan Osman <nathan@quickmediasolutions.com>"

# Install postgresql-dev so that psycopg2 can be built; then remove it
RUN \
    apk add --no-cache postgresql-dev && \
    pip3 install --no-cache-dir psycopg2 && \
    apk del postgresql-dev
