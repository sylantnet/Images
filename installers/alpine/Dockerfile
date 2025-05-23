FROM --platform=$TARGETOS/$TARGETARCH alpine:latest

LABEL author="Sabrina Goom" maintainer="sabrina@sylant.net"

LABEL org.opencontainers.image.source="https://github.com/sylantnet/images"
LABEL org.opencontainers.image.licenses=MIT

ENV DEBIAN_FRONTEND=noninteractive

RUN apk add --update --no-cache ca-certificates curl git jq wget