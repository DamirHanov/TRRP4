FROM golang:1.14

ARG PORT=3000

COPY . .

ENV TRRP4_CROP_ADDR 127.0.0.1:$PORT

EXPOSE $PORT

RUN go get -v github.com/golang/protobuf/proto
RUN go build -o main .

CMD ["./main"]
