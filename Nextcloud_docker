#!/bin/bash

# Обновление списка пакетов
sudo apt update

# Установка Docker
sudo apt install -y docker.io

# Запуск Docker
sudo systemctl start docker

# Включение Docker при загрузке
sudo systemctl enable docker

# Создание директории для данных Nextcloud
mkdir nextcloud_data
cd nextcloud_data

# Запуск контейнера Docker для Nextcloud
sudo docker run -d --name nextcloud -p 8080:80 -v $PWD:/var/www/html nextcloud
