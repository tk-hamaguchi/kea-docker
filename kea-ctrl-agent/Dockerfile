FROM alpine:3.14

ENV KEA_VERSION 1.8.2-r5
ENV CONF_FILE /etc/kea/kea-ctrl-agent.conf

RUN apk add kea-ctrl-agent=${KEA_VERSION}

RUN mkdir -p /run/kea

CMD kea-ctrl-agent -c ${CONF_FILE}
