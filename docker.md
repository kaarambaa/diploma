# Docker

 Чтобы запустить приложение в контейнере Docker, вам прежде всего понадобится создать Docker image используя `Dockerfile`. Поэтому, создадим два `Dockerfile`, по одному для каждой директории проекта.

 ## Docker images
 
 Чтобы получить необходимые зависимости, нам нужно выполнить следующискрипт:
 ```
 coffee-shop/liberty/prepare.sh
 barista/liberty/prepare.sh
 ```
 Давайте начнем с приложения coffee-shop. Под `coffee-shop/` мы создадим `Dockerfile` со следующим содержимым:
 ```
 FROM open-liberty:20.0.0.3-full-java8-openj9

 COPY liberty/extension /liberty/usr/extension/
 COPY liberty/server.xml /config/

 COPY target/coffee-shop.war /config/dropins/
 ```
 

