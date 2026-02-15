FROM        --platform=$TARGETOS/$TARGETARCH ubuntu:24.04

LABEL       author="Lucas Mcginnis" maintainer="lucas.mcginnis@lrmtheboss.com"

LABEL       org.opencontainers.image.source="https://github.com/lrmtheboss/BossDockerImages"
LABEL       org.opencontainers.image.licenses=MIT

ENV         DEBIAN_FRONTEND=noninteractive

RUN         apt update \
						&& apt upgrade -y \
						&& apt -y --no-install-recommends install ca-certificates curl git unzip zip tar jq wget
