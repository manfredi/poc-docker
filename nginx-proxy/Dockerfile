# docker build --no-cache -t poc-nginx-proxy:latest .
# docker run -d --name poc-nginx-proxy --rm -p 80:80  poc-nginx-proxy:latest

FROM nginx:1.23.3
COPY ./default.conf  /etc/nginx/conf.d/default.conf
EXPOSE 80
