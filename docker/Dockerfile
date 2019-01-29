FROM debian:9
COPY 99fixbadproxy /etc/apt/apt.conf.d/
RUN apt update
RUN apt upgrade -y
RUN apt install nginx -y
RUN which nginx
ENTRYPOINT ["nginx"]
CMD ["-g", "daemon off;"]