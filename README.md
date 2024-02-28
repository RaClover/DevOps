1. a bash script that will create
a separate folder in the root directory with the user name for all users of the system and
set the rights 755 for it. In this case, the owner of the folder must be the corresponding user.
The path to the root directory of the directory creation must be determined when the script is run by the user.
The log should be written both to stdout and to a file.<br><br><br>



2. Dockerfile для создания образа, который будет поддерживать веб-сервер Apache или Nginx и базу данных MySQL . В Dockerfile дополнительные возможности использования: FROM, MAINTAINER, RUN, CMD, WORKDIR, ENV, add, Copy, VOLUME, USER, EXPOSE.<br><br><br><br>



3. docker to compose a config for deploying two containers on the same network (10.10.10.0/28) of the bridge type: 1 - Nginx or Apache server, then volume configuration files should be transmitted to it, port 80 from the container should be available on the host machine via port 8080 2 - MySQL , and the data storage directory should be mounted as volume settings, volume settings should be described in the same docker-compose configuration file. The break with the database should be unavailable due to the contact server with the web server named new_db, dev_db.
