FROM node:5.11

RUN apt-get update && \
    apt-get install -y \
        ssh \
        && \
    apt-get clean

RUN mkdir -p /var/www/dobot && \
    chown 1000:1000 /var/www/dobot

COPY docker-entrypoint.sh /usr/local/bin

EXPOSE 22

ENTRYPOINT ["docker-entrypoint.sh"]
CMD ["/usr/sbin/sshd","-D"]
VOLUME ["/var/www/dobot"]
