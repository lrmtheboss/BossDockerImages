# ----------------------------------
# Environment: MongoDB
# ----------------------------------
FROM        --platform=$TARGETOS/$TARGETARCH mongo:7-jammy

LABEL       author="Lucas Mcginnis" maintainer="lucas.mcginnis@lrmtheboss.com"

ENV         DEBIAN_FRONTEND noninteractive

RUN         apt update -y && apt install -y netcat iproute2
RUN         useradd -d /home/container -m container -s /bin/bash

USER        container
ENV         USER=container HOME=/home/container
WORKDIR     /home/container

COPY        ./entrypoint.sh /entrypoint.sh
CMD ["/bin/bash", "/entrypoint.sh"]
