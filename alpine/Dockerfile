FROM alpine:latest

RUN apk update \
    && apk upgrade \
    && apk add \
    	ca-certificates \
	wget \
    && rm -rf /var/cache/apk/*

RUN cd /usr/local/share/ca-certificates \
    && wget https://pki.jlab.org/JLabCA.crt \
    && update-ca-certificates
