FROM golang:1.20

RUN apt update && apt install -y protobuf-compiler 

WORKDIR /go

COPY Makefile .

ENV TZ=Asia/Shanghai
ENV GOPROXY=https://goproxy.cn,https://goproxy.io,direct


RUN make init && rm -rf ./Makefile

RUN git clone https://github.com/confluentinc/librdkafka.git && \
    cd librdkafka && \
    ./configure && \
    make && \
    make install
