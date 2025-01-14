FROM ubuntu:24.04

RUN apt-get update && \
  apt-get install -y gcc python-dev libkrb5-dev && \
  apt-get install -y python3-pip && \
  pip3 install --upgrade  pip && \ 
  pip3 install --upgrade virtualenv && \ 
  pip3 install pywinrm[kerberos] && \
  apt install -y krb5-user && \
  pip3 install pywinrm && \ 
  pip3 install ansible
