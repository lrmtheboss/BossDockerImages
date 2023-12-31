FROM        --platform=$TARGETOS/$TARGETARCH bellsoft/liberica-openjdk-alpine:8

LABEL       author="Lucas Mcginnis" maintainer="lucas.mcginnis@lrmtheboss.com"

LABEL       org.opencontainers.image.source="https://github.com/lrmtheboss/docker-images"
LABEL       org.opencontainers.image.licenses=MIT

RUN         apk update && apk upgrade && \
            apk add --no-cache \
            bash \
            curl \
            wget \
            lsof \
            ca-certificates \
            tar \
            sqlite3 \
            fontconfig \
            tzdata \
            iproute2 \
            libfreetype6 \
            tini \
            && apk cache clean

## Setup user and working directory
RUN         adduser -h /home/container -d -s /bin/bash container
USER        container
ENV         USER=container HOME=/home/container
WORKDIR     /home/container

STOPSIGNAL SIGINT

COPY        --chown=container:container ./../entrypoint.sh /entrypoint.sh
RUN         chmod +x /entrypoint.sh
ENTRYPOINT    ["/usr/bin/tini", "-g", "--"]
CMD         ["/entrypoint.sh"]