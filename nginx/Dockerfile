FROM nginx

RUN rm -rf /docker-entrypoint.d/10-listen-on-ipv6-by-default.sh

COPY nginx.conf /etc/nginx/nginx.conf
COPY conf.d/blogod.conf /etc/nginx/conf.d/

STOPSIGNAL SIGQUIT

CMD ["nginx", "-g", "daemon off;"]

