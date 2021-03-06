# Введение

В рамках данного воркшопа мы разберем, как, ипользуя Jakarta EE и MicroProfile, можно разрабатывать облачные микросервисы, которые могут быть развернуты с использованием Docker, Kubernetes и Istio. Мы рассмотрим основы современных Enterprise Java-сервисов, а также их масштабируемость, отказоустойчивость, наблюдаемость, маршрутизацию трафика и конечно же их настройку.

## Пример решения

Для иллюстрации мы будем использовать два микросервиса: *coffee-shop* и *barista*, оба из которых разработаны как enterprise-приложения на Jakarta EE и MicroProfile. Оба сервиса развернуты полностью независимо друг от друга и связываются посредством HTTP (REST) запросов.

Приложения развернуты на OpenLiberty - open-source сервере, который поддерживает множество различных Java технологий, включая Jakarta и MircoProifle.

## Начало

Чтобы начать, склонируйте Git репозиторий и откройте проекты, находящиеся в нем:
```
git clone https://github.com/sdaschner/cloud-native-workshop-02-2020
cd cloud-native-workshop-02-2020/
``` 
## Создание

Наши приложения построены с использованием Maven. Оба микросервисных проекта содержат файл pom.xml, который определяет конфигурацию сборки проекта и его зависимостей.

Для начала мы создаем оба приложения микросервиса, перейдя в соответствующие каталоги и выполнив команду сборки Maven:
```
cd coffee-shop/
mvn package

cd ../barista/
mvn package
```
Эти две команды позволят вам создать оба приложения, используя Maven `package phase`. В результате работы команду у вас появяься WAR файлы: `coffee-shop.war` и `barista.war`, содержащие в себе наши приложения, которые в последствии будут развернуты в контейнерах. 

## Запуск

Для запуска приложений, мы могли бы развернуть их в работающих локально контейнерах. Однако поскольку мы нацелены на работу в облаке, будем разворачивать их в виде Linux контейнеров, используя Docker.

Чтобы запустить Docker-контейнеры, необходимо создать соответсвующие образы Docker, содержащие всё, что нужно для запуска и функционирования наших приложений.

Теперь, давайте посмотрим, как можно сделать (это)[]