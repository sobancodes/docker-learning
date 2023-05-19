FROM nginx:stable-alpine

RUN mkdir -p /var/www/html

COPY nginx.conf /etc/nginx/conf.d/default.conf

COPY index.html /var/www/html/public/index.html

RUN sed -i "s/user www-data/user laravel/g" /etc/nginx/nginx.conf

RUN adduser -g laravel -s /bin/sh -D laravel

EXPOSE 8000