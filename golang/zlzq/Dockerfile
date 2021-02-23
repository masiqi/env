FROM golang:1.15.5-buster

ENV GOPROXY https://goproxy.cn,direct
ENV GO111MODULE on

WORKDIR /go/cache

ADD data/go.mod .
ADD data/go.sum .
RUN go mod download

WORKDIR /go/release

ADD . .
