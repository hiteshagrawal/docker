FROM nginx 
MAINTAINER Hitesh Agrawal "hitesh_a2003@yahoo.com"
#RUN mkdir /etc/nginx/logs && touch /etc/nginx/logs/static.log
#RUN mkdir /www
ADD ./default.conf /etc/nginx/conf.d/default.conf
ADD ./index.html /usr/share/nginx/html/
#VOLUME ["/usr/share/nginx/html", "/var/log/nginx/log"]
#EXPOSE 80
#EXPOSE 443
#CMD "echo" "Hello docker! Welcome to the nginx server installed by hitesh"
#CMD nginx
#MAINTAINER NGINX Docker Maintainers "docker-maint@nginx.com"
#RUN apt-key adv --keyserver hkp://pgp.mit.edu:80 --recv-keys 573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62
#RUN echo "deb http://nginx.org/packages/mainline/debian/ jessie nginx" >> /etc/apt/sources.list
#ENV NGINX_VERSION=1.9.6-1~hitesha
#RUN apt-get update && apt-get install -y ca-certificates nginx=${NGINX_VERSION} && rm -rf /var/lib/apt/lists/*
#RUN ln -sf /dev/stdout /var/log/nginx/access.log
#RUN ln -sf /dev/stderr /var/log/nginx/error.log
VOLUME /var/cache/nginx /usr/share/nginx/html /var/log/nginx/log
EXPOSE 443/tcp 80/tcp
CMD "nginx" "-g" "daemon off;"
