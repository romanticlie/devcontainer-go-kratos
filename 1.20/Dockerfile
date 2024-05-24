FROM golang:1.20

RUN apt update && apt install -y protobuf-compiler clang-format

WORKDIR /go

COPY Makefile .

ENV TZ=Asia/Shanghai
ENV GOPROXY=https://goproxy.cn,https://goproxy.io,direct


RUN make init && rm -rf ./Makefile
