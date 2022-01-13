FROM ubuntu:20.04

MAINTAINER wangjunkang <wangjunkangha@163.com>

RUN apt update \
    && apt install python2.7 -y \
    && cp /usr/bin/python2.7 /usr/bin/python \
    && apt install wget -y \
    && mkdir -p /data/{job,env} && cd /data \
    && wget "https://bootstrap.pypa.io/pip/2.7/get-pip.py" -O get-pip.py \
    && python get-pip.py && rm -rf get-pip.py

WORKDIR /data/job

CMD ["tail", "-f", "/dev/null"]
