FROM debian:wheezy

RUN apt-get update && apt-get -yq install curl unzip sqlite3 libsqlite3-dev build-essential && \
  curl -sL https://deb.nodesource.com/setup | bash - && \
  apt-get install -y nodejs

# GHOST
RUN mkdir -p /app && \
  cd /tmp && \
  curl -L -o ghost-latest.zip https://ghost.org/zip/ghost-latest.zip && \
  unzip ghost-latest.zip -d /app && \
  rm -f ghost-latest.zip && \
  npm install --production --prefix /app

ADD config.js /app/

WORKDIR /app
EXPOSE 2368

ENV GHOST_URL https://www.brianchristner.io
VOLUME ["/app/content/data"]
CMD ["node", "index.js"]
