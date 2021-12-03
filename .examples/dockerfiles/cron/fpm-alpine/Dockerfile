FROM nextcloud:fpm-alpine

RUN apk add --no-cache supervisor

COPY supervisord.conf /

ENV NEXTCLOUD_UPDATE=1

CMD ["/usr/bin/supervisord", "-c", "/supervisord.conf"]
