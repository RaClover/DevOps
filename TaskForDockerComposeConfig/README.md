# Task docker compose config, to deploy two containers on the same network (10.10.10.0/28) of the bridge type


## Project Overview

Напишите docker compose конфиг, для разворачивания двух контейнеров в одной сети (10.10.10.0/28) типа bridge: 
1 - Nginx или Apache, ему должны передаваться конфигурационные файлы через volume, порт 80 из контейнера должен быть доступен на хостовой машине по порту 8080
2 - mysql или postgres, каталог для хранения данных должен монтироваться как docker volume, docker volume должен быть описан в том же конфигурационном файле docker compose. Сервис с БД должен быть доступен из контейнера с веб-сервером по именам new_db, dev_db.<br><br><br><br>




Write a docker compose config, to deploy two containers on the same network (10.10.10.0/28) of the bridge type:
1 - Nginx or Apache, configuration files should be transferred to it via volume, port 80 from the container should be available on the host machine on port 8080
2 - mysql or postgres, the data storage directory should be mounted as docker volume, docker volume should be described in the same docker compose configuration file. The service with the database must be accessible from the container with the web server by the names new_db, dev_db.<br><br><br>
  
  
  ## Использование
 
  1. Создал docker-compose.yml с вышеуказанным содержимым.
  
  2. Создал html-каталог, внутри которого создал index.html и style.css.
 3. Запустил контейнеры с помощью Docker Compose: docker-compose up
4. откройте http://localhost:8080 мы увидим, что содержимое, которое находится внутри html
  
  
  
  
  ## Usage
 
  1. Created docker-compose.yml wiht the above content.
  
  2. Created html derectory inside it created an index.html and style.css.
 3. Started the containers using Docker Compose: docker-compose up
4. open http://localhost:8080 we will see the the content that is inside the html



