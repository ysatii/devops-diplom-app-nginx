FROM nginx:1.27-alpine

# Кладём статический сайт
COPY index.html /usr/share/nginx/html/index.html

# Подменяем конфиг nginx
COPY nginx.conf /etc/nginx/conf.d/default.conf

EXPOSE 80
