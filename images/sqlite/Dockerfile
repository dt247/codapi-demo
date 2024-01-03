FROM alpine:3.19

RUN apk update && apk upgrade && apk add sqlite

RUN adduser --home /sandbox --disabled-password sandbox

USER sandbox
WORKDIR /sandbox
