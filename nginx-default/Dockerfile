FROM ubuntu:14.04
MAINTAINER Hitesh Agrawal "hitesh_a2003@yahoo.com"
RUN apt-get update
RUN apt-get install -y nginx
RUN echo -e "Our first Docker image for Nginx `uname -n`" > /usr/share/nginx/html/index.html
#VOLUME /var/cache/nginx /usr/share/nginx/html /var/log/nginx/log
RUN ln -sf /dev/stdout /var/log/nginx/access.log
RUN ln -sf /dev/stderr /var/log/nginx/error.log
CMD "nginx" "-g" "daemon off;"
EXPOSE 80
