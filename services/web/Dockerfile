FROM nginx:1.15.12-alpine

RUN apk add --no-cache bash certbot certbot-nginx esh && \
    rm /etc/nginx/conf.d/default.conf

COPY ./conf/nginx.conf /etc/nginx/
COPY ./conf/conf.d/* /etc/nginx/conf.d/
COPY bin/* /maison/bin/
RUN chmod ug+rx /maison/bin/*

CMD ["/maison/bin/entry-point"]

EXPOSE 80 443
