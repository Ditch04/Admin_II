FROM nginx

COPY nginx.conf /etc/nginx/nginx.conf

RUN apt update && apt install -y certbot python3-certbot-nginx
RUN certbot --nginx -n -d www.l1-8.ephec-ti.be | echo "1"

EXPOSE 80
EXPOSE 443


