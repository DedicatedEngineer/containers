FROM ubuntu:24.04

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && \
  apt-get install -y gcc python3 libkrb5-dev && \
  apt-get install -y python3-pip python3.12-venv && \
  apt-get install -y ssh && \
  python3 -m venv .venv && \
  .venv/bin/pip3 install --upgrade  pip && \ 
  .venv/bin/pip3 install --upgrade virtualenv && \ 
  .venv/bin/pip3 install pywinrm[kerberos] && \
  apt-get install -y krb5-user && \
  .venv/bin/pip3 install pywinrm && \ 
  .venv/bin/pip3 install ansible
