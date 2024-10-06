FROM        --platform=$TARGETOS/$TARGETARCH alpine:latest

LABEL       author="Lucas Mcginnis" maintainer="lucas.mcginnis@lrmtheboss.com"

LABEL       org.opencontainers.image.source "https://github.com/lrmtheboss/BossDockerImages"
LABEL       org.opencontainers.image.licenses=MIT

RUN         apk add --update --no-cache ca-certificates tzdata tini
RUN         adduser -D -h /home/container container

USER        container
ENV         USER=container HOME=/home/container
WORKDIR     /home/container

STOPSIGNAL SIGINT

COPY        --chown=container:container ./entrypoint.sh /entrypoint.sh
RUN         chmod +x /entrypoint.sh
ENTRYPOINT    ["/sbin/tini", "-g", "--"]
CMD         ["/entrypoint.sh"]