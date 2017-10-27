FROM nginx:1.9
MAINTAINER Nick Janetakis <nick.janetakis@gmail.com>

#RUN rm /usr/share/nginx/html/*

COPY configs/nginx.conf /etc/nginx/nginx.conf

CMD ["nginx", "-g", "daemon off;"]