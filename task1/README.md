Создание образа
docker build -t hw-nginx:first .

Запуск контейнера:
docker run -it --rm -d -p 8081:80 hw-nginx:first

Проверка сайта:
curl localhost:8081

Узнать ID контейнера
docker ps

Остановка контейнера:
docker stop <ID контейнера>
