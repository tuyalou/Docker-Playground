FROM ubuntu:xenial
LABEL maintainer="tuubayalcin@gmail.com"
RUN apt-get update && apt-get install nginx -y
RUN ln -sf /dev/stdout /var/log/nginx/access.log && ln -sf /dev/stderr /var/log/nginx/error.log
EXPOSE 80
CMD ["/usr/sbin/nginx", "-g", "daemon off;"]
