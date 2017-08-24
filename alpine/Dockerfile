FROM alpine:latest

ENV http_proxy=http://jprox.jlab.org:8081 \
    https_proxy=https://jprox.jlab.org:8081

RUN apk update \
    && apk upgrade \
    && apk add \
    	ca-certificates \
	wget \
    && rm -rf /var/cache/apk/*

RUN cd /usr/local/share/ca-certificates \
    && wget https://pki.jlab.org/JLabCA.crt \
    && update-ca-certificates
