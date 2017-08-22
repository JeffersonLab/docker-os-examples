FROM debian:jessie

ENV http_proxy=http://jprox.jlab.org:8081 \
    https_proxy=https://jprox.jlab.org:8081

RUN apt-get update && apt-get upgrade \
    && apt-get install -y \
       	curl

RUN cd /usr/local/share/ca-certificates \
    && curl -sLO https://pki.jlab.org/JLabCA.crt \
    && update-ca-certificates

