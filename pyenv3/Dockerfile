FROM ubuntu:20.04

MAINTAINER wangjunkang <wangjunkangha@163.com>

RUN apt update \
    && apt install python3-pip -y \
    && cp /usr/bin/python3 /usr/bin/python \
    && mkdir -p /data/{job,env} && cd /data

WORKDIR /data/job

CMD ["tail", "-f", "/dev/null"]
