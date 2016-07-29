FROM node:6.3

MAINTAINER David Barker <david.barker@givesmart.com>

RUN apt-get update && apt-get install -y --force-yes \
        sqlite3 \
        libsqlite3-dev

# Clean up
RUN apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

WORKDIR /var/www/sass

CMD [ "npm", "start" ]