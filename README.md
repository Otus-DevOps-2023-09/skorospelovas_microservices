# skorospelovas_microservices
skorospelovas microservices repository

ДЗ №1  Docker контейнеры. Docker под капотом
1. Подготовлен файл Dockerfile и создан образ reddit
2. Создан инстанс в yc
3. Развернут образ reddit в созданом инстансе
4. Образ сохранен на hub.docker.com
Для запуска сборки образа необходимо зайти в папку docker-monolith и выполнить команду
```
docker build -t reddit:latest .
```

Для запуска приложения необходимо выполнить команду
```
docker run -d -p 9292:9292 --name reddit reddit:latest
```

Для проверки работоспособности необходимо зайти на адрес http://<ip адрес>:9292
