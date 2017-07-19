FROM golang:1.8.3-alpine

ENTRYPOINT ["/go/bin/godoc"]
CMD ["-http=:6060"]

EXPOSE 6060

RUN apk --no-cache add git &&\
    go get golang.org/x/tools/cmd/godoc &&\
    apk del git
