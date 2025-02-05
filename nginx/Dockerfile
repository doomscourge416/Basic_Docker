FROM ubuntu:latest

# Обновляем пакеты и устанавливаем Nginx
RUN apt-get update && \
    apt-get install -y nginx && \
    rm -rf /var/lib/apt/lists/*

# Удаляем дефолтный сайт
RUN rm /etc/nginx/sites-enabled/default

# Рабочая директория
WORKDIR /data

VOLUME /data

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]