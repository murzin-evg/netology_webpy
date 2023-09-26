Создание образа docker build -t hw-django:first .

Запуск контейнера: docker run -it --rm -d -p 8081:80 hw-django:first

Проверка сайта через терминал: curl localhost:8081/api/v1

Примеры запросов в файле requests-examples.http

Узнать ID контейнера docker ps

Остановка контейнера: docker stop <ID контейнера>

