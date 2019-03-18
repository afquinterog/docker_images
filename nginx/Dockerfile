FROM nginx:1.9
MAINTAINER Andres Quintero <andres@venture.co>

RUN rm /usr/share/nginx/html/*

COPY configs/nginx.conf /etc/nginx/nginx.conf
COPY configs/default.conf /etc/nginx/conf.d/default.conf

COPY docker-entrypoint /
RUN chmod +x /docker-entrypoint
ENTRYPOINT ["/docker-entrypoint"]

CMD ["nginx", "-g", "daemon off;"]