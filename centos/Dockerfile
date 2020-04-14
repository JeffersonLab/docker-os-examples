FROM centos:centos7

RUN cd /etc/pki/ca-trust/source/anchors \
    && curl -sLO https://pki.jlab.org/JLabCA.crt \
    && update-ca-trust \
    && yum update -y \
    && yum clean all
