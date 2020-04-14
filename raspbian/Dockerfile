FROM arm32v7/debian:jessie

RUN apt-get update && apt-get upgrade \
    && apt-get install -y \
       	curl

RUN cd /usr/local/share/ca-certificates \
    && curl -sLO https://pki.jlab.org/JLabCA.crt \
    && update-ca-certificates

