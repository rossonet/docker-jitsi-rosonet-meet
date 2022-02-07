ARG JITSI_REPO=image-registry.openshift-image-registry.svc:5000/jitsi-dev
ARG BASE_TAG=latest
FROM ${JITSI_REPO}/jitsi-rossonet-base-java:${BASE_TAG}

RUN apt-dpkg-wrap apt-get update && \
    apt-dpkg-wrap apt-get install -y jitsi-videobridge2 jq curl iproute2 dnsutils && \
    apt-cleanup

COPY rootfs/ /

VOLUME /config
