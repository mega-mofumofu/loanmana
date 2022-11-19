FROM golang:1.19-alpine

WORKDIR /go/src
COPY ./loanmana/src .

RUN apk update \
  && apk add --no-cache git \
  && go get github.com/gin-gonic/gin \
  && go get github.com/jinzhu/gorm \
  && go get github.com/go-sql-driver/mysql

EXPOSE 8080

