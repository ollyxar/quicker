FROM nginx:alpine

RUN apk update && apk add openssl
RUN openssl req \
        -new \
        -newkey rsa:2048 \
        -days 365 \
        -nodes \
        -x509 \
        -subj "/C=UA/ST=Kyiv/L=Kyiv/O=Org/CN=localhost" \
        -keyout /etc/nginx/conf.d/server.key \
        -out /etc/nginx/conf.d/server.crt

RUN cat /etc/nginx/conf.d/server.crt /etc/nginx/conf.d/server.key > /etc/nginx/conf.d/server.pem