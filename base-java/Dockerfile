ARG JITSI_REPO=jitsi-dev
ARG BASE_TAG=latest
FROM ${JITSI_REPO}/jitsi-rossonet-base:${BASE_TAG}

RUN mkdir -p /usr/share/man/man1 && \
    apt-dpkg-wrap apt-get update && \
    apt-dpkg-wrap apt-get install -y openjdk-11-jre-headless && \
    apt-cleanup
