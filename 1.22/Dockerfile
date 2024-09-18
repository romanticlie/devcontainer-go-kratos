FROM golang:1.22.6

RUN apt update \
     && apt install -y --no-install-recommends \
     protobuf-compiler \
     ca-certificates  \
     netbase \
     curl \
     procps \
     iproute2 \
     iputils-ping \
     sysstat \
     clang-format


WORKDIR /go

COPY Makefile .

ENV TZ=Asia/Shanghai
ENV GOPROXY=https://goproxy.cn,https://goproxy.io,direct


RUN make init && rm -rf ./Makefile
