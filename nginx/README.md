# Nginx

## Build

```sh
$ cd docky/nginx
$ docker build -t hulz413/nginx .
```

## Run

```sh
$ docker run --name nginx \
        --add-host host.docker.internal:host-gateway \
        -v /home/hulz/projects/nginx/logs:/var/log/nginx \
        -p 80:80 \
        --restart always \
        -d \
        hulz413/nginx
```
