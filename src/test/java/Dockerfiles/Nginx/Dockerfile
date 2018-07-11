FROM nginx:alpine

USER root

ENV NGINX_HOST=foobar.com
ENV NGINX_PORT=80

COPY default.conf /etc/nginx/conf.d/
COPY index.html /usr/share/nginx/html/

VOLUME /usr/share/nginx/html
VOLUME /etc/nginx

EXPOSE 80

#CMD ['nginx', '-g', 'daemon off;'] or -->  exec nginx-debug -g 'daemon off;'
CMD nginx-debug -g 'daemon off;'