FROM ubuntu:latest
RUN apt-get update
RUN apt-get install -y nginx
COPY ./config/entry.local.conf /etc/nginx/sites-enabled/entry.local.conf
WORKDIR /data/app
VOLUME /data/app
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]