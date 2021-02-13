FROM nginx:stable

RUN apt-get update

RUN ln -sf /dev/stdout /var/log/nginx/access.log \
    && ln -sf /dev/stderr /var/log/nginx/error.log

COPY ./docker/web/nginx/nginx.conf /etc/nginx/nginx.conf
COPY ./docker/web/nginx/conf.d/* /etc/nginx/conf.d/

COPY ./docker/web/run.sh /tmp
RUN ["chmod", "+x", "/tmp/run.sh"]
CMD ["/tmp/run.sh"]