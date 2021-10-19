# https://github.com/docker-library/httpd/issues/165
# https://hub.docker.com/_/debian
# https://hub.docker.com/_/httpd
# https://github.com/docker-library/httpd
FROM debian:bullseye

RUN apt update && apt install -y --no-install-recommends apache2 libapache2-mod-jk

EXPOSE 80 443

CMD ["apachectl", "-k", "start", "-DFOREGROUND"]