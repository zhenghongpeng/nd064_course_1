FROM golang:alpine
ENV CGO_ENABLED=0 
ENV GOOS=linux 
ENV GO111MODULE=on

WORKDIR /go/src/app

ADD . .

RUN go build -mod=vendor -a  -o helloworld main.go

EXPOSE 6111

CMD ["./helloworld"]