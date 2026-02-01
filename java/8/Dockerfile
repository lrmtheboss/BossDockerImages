FROM        --platform=$TARGETOS/$TARGETARCH bellsoft/liberica-openjdk-alpine-musl:8

LABEL       author="Lucas Mcginnis" maintainer="lucas.mcginnis@lrmtheboss.com"

LABEL       org.opencontainers.image.source="https://github.com/lrmtheboss/BossDockerImages"
LABEL       org.opencontainers.image.licenses=MIT

RUN         apk update && apk upgrade && \
            apk add --no-cache \
            bash \
            curl \
            wget \
            lsof \
            ca-certificates \
            tar \
            fontconfig \
            tzdata \
            iproute2 \
            tini \
            eudev-libs \
            freetype \
            gcc \
            libstdc++ \
            font-jetbrains-mono \
            && apk cache clean

RUN         adduser -h /home/container -D -s /bin/bash container
USER        container
ENV         USER=container HOME=/home/container
WORKDIR     /home/container

STOPSIGNAL SIGINT

COPY        --chown=container:container ./../entrypoint.sh /entrypoint.sh
RUN         chmod +x /entrypoint.sh
ENTRYPOINT    ["/sbin/tini", "-g", "--"]
CMD         ["/bin/bash", "/entrypoint.sh"]