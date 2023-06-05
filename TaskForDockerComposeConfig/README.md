# Task docker compose config, to deploy two containers on the same network (10.10.10.0/28) of the bridge type


## Project Overview

Напишите docker compose конфиг, для разворачивания двух контейнеров в одной сети (10.10.10.0/28) типа bridge: 
1 - Nginx или Apache, ему должны передаваться конфигурационные файлы через volume, порт 80 из контейнера должен быть доступен на хостовой машине по порту 8080
2 - mysql или postgres, каталог для хранения данных должен монтироваться как docker volume, docker volume должен быть описан в том же конфигурационном файле docker compose. Сервис с БД должен быть доступен из контейнера с веб-сервером по именам new_db, dev_db.<br><br><br><br>




Write a docker compose config, to deploy two containers on the same network (10.10.10.0/28) of the bridge type:
1 - Nginx or Apache, configuration files should be transferred to it via volume, port 80 from the container should be available on the host machine on port 8080
2 - mysql or postgres, the data storage directory should be mounted as docker volume, docker volume should be described in the same docker compose configuration file. The service with the database must be accessible from the container with the web server by the names new_db, dev_db.<br><br><br>
  
  
  
  
  
  ## Usage
 
  1. Created Dockerfile wiht the above content.
  
  2. Created config.php file for database (mysql) configration.
  3. Created index.html
  4. run docker build -t raheeb_image_$(date)  in the terminal to  build the Docker image using the Dockerfile in the current directory (.) and tag it with the name raheeb_image_<current date>. The $(date +%Y-%m-%d) part dynamically adds the current date to the image name.
  
  5. run docker images in the terminal to see the newly created image, raheeb_image_<current date>, listed in the output.



