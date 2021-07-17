# Build

```sh
$ cd docky/shadowsocks
$ docker build -t go-shadowsocks2 .
```

# Run

```sh
$ docker run -d --restart=always --name=shadowsocks -p 8388:8388 -e PASSWORD=123456 go-shadowsocks2:latest
```
