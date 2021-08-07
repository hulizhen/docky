# Shadowsocks

## Build

```sh
$ cd docky/shadowsocks
$ docker build -t hulz413/shadowsocks .
```

## Push

$ docker push hulz413/shadowsocks

## Pull

```sh
$ docker pull hulz413/shadowsocks
```

## Run

```sh
$ docker run -d \
        --restart always \
        --name=shadowsocks \
        -p 8388:8388 \
        -e PASSWORD=123456 \
        hulz413/shadowsocks
```
