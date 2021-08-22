FROM alpine:3.14

ENV KEA_VERSION 1.8.2-r5
ENV CONF_FILE /etc/kea/kea-dhcp4.conf

RUN apk add kea=${KEA_VERSION}
RUN apk add mysql-dev mysql-client

RUN mkdir -p /run/kea

CMD kea-dhcp4 -c ${CONF_FILE}
