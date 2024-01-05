FROM golang:1.16.8-bullseye

WORKDIR /usr/src/app

EXPOSE 8080

COPY go.mod ./
COPY go.sum ./
COPY *.go ./
COPY router/ ./router/
COPY pgconnection/ ./pgconnection/
COPY cache/ ./cache/
COPY common/ ./common/
COPY controller/ ./controller/

RUN go build

CMD ["go", "test", "./..."]
