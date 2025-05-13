FROM debian:bullseye

RUN apt update -y && apt upgrade -y && apt install -y php php-fpm

RUN mkdir -p /run/php

COPY www.conf /etc/php/7.4/fpm/pool.d/.

CMD ["/usr/sbin/php-fpm7.4", "-F"]
