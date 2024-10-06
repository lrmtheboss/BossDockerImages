# ----------------------------------
# Environment: redis
# ----------------------------------
FROM    --platform=$TARGETOS/$TARGETARCH redis:7-alpine

LABEL   author="Lucas Mcginnis" maintainer="lucas.mcginnis@lrmtheboss.com"

ENV     DEBIAN_FRONTEND noninteractive

RUN     apk update && \
        apk upgrade && \
        apk add --no-cache iproute2 \
        && apk cache clean

RUN     useradd -d /home/container -m container -s /bin/bash

USER    container
ENV     USER=container HOME=/home/container
WORKDIR /home/container

COPY    ./entrypoint.sh /entrypoint.sh
CMD     ["/bin/bash", "/entrypoint.sh"]