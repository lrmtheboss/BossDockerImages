FROM        --platform=$TARGETOS/$TARGETARCH node:20-alpine

LABEL       author="Lucas Mcginnis" maintainer="lucas.mcginnis@lrmtheboss.com"

RUN         apk update && apk upgrade
RUN         apk add --no-cache ffmpeg iproute2 git sqlite python3 python3-dev ca-certificates tzdata zip tar curl libtool iputils-ping tini
RUN         adduser -h /home/container -D -s /bin/bash container

RUN         npm install npm@latest typescript ts-node @types/node --location=global

# install pnpm
RUN         npm install -g corepack
RUN         corepack enable
RUN         corepack prepare pnpm@latest --activate

USER        container
ENV         USER=container HOME=/home/container
WORKDIR     /home/container

STOPSIGNAL SIGINT

COPY        --chown=container:container ./../entrypoint.sh /entrypoint.sh
RUN         chmod +x /entrypoint.sh
ENTRYPOINT    ["/usr/bin/tini", "-g", "--"]
CMD         ["/entrypoint.sh"]