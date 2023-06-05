# Task for doccker image usign apache and mysql


## Project Overview

Напишите Dockerfile для создания образа, который будет содержать веб-сервер Apache или Nginx и базу данных MySQL или postgresql. В Dockerfile должны использоваться инструкции: FROM, MAINTAINER, RUN, CMD, WORKDIR, ENV, ADD, COPY, VOLUME, USER, EXPOSE.
Dockerfile должен содержать комментарии с пояснениями того, что делается. 
Собранный образ должен иметь имя вида <фамилия>_<инициалы>_image_<текущая дата>. Рядом с dockerfile должен быть скрин, на котором будут видны все слои вашего image и их размер на диске, команда, которой вы это выведете.<br><br><br><br>




Write a Dockerfile to create an image that will contain an Apache or Nginx web server and a MySQL or postgresql database. The following instructions should be used in the Dockerfile: FROM, MAINTAINER, RUN, CMD, WORKDIR, ENV, ADD, COPY, VOLUME, USER, EXPOSE.
The dockerfile should contain comments explaining what is being done.
The assembled image must have a name of the form <surname>_<initials>_image_<current date>. Next to the dockerfile there should be a screen on which all the layers of your image and their size on disk will be visible, the command that you will output it to.<br><br><br>
  
  
  
  
  
  ## Usage
 
  1. Created Dockerfile wiht the above content.
  
  2. Created config.php file for database (mysql) configration.
  3. Created index.html
  4. run docker build -t raheeb_image_$(date)  in the terminal to  build the Docker image using the Dockerfile in the current directory (.) and tag it with the name raheeb_image_<current date>. The $(date +%Y-%m-%d) part dynamically adds the current date to the image name.
  
  5. run docker images in the terminal to see the newly created image, raheeb_image_<current date>, listed in the output.



