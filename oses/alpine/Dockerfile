FROM --platform=$TARGETOS/$TARGETARCH alpine:latest

LABEL author="Sabrina Goom" maintainer="sabrina@sylant.net"

LABEL org.opencontainers.image.source="https://github.com/sylantnet/images"
LABEL org.opencontainers.image.licenses=MIT

RUN apk add --update --no-cache ca-certificates tzdata \
        && adduser -D -h /home/container container

USER container
ENV USER=container HOME=/home/container

WORKDIR /home/container

COPY ./entrypoint.sh /entrypoint.sh
CMD [ "/bin/ash", "/entrypoint.sh" ]