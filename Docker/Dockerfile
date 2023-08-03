FROM golang:1.20 as developer

WORKDIR /app

FROM developer as prod

WORKDIR /go/src/relay
COPY ./ .

RUN go build -o relay cmd/main.go