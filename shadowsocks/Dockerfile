FROM golang:1.16

RUN go get github.com/shadowsocks/go-shadowsocks2

ENV CIPHER=AEAD_AES_256_GCM
ENV PASSWORD=123456
ENV SERVER_PORT=8388

EXPOSE ${SERVER_PORT}
CMD exec go-shadowsocks2 -verbose -s "ss://${CIPHER}:${PASSWORD}@:${SERVER_PORT}"
