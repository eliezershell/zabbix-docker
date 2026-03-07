FROM nginx:1.29.5@sha256:0236ee02dcbce00b9bd83e0f5fbc51069e7e1161bd59d99885b3ae1734f3392e
COPY default.conf /etc/nginx/conf.d/default.conf
COPY certs/cert.pem /etc/ssl/certs/cert.pem
COPY certs/privkey.pem /etc/ssl/private/privkey.pem
