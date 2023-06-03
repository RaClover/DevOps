# Use a base image
FROM ubuntu:latest

# Maintainer information
MAINTAINER Raheeb <Raheeb772652540@gmail.com>

# Update the package manager and install dependencies
RUN apt-get update \
    && apt-get install -y apache2 mysql-server

# Set the working directory
WORKDIR /var/www/html

# Set environment variables if needed
ENV DATABASE_HOST=localhost \
    DATABASE_PORT=3306

# Add files from the host to the container
COPY config.php /var/www/html/config.php

# Copy files from the host to the container
COPY index.html /var/www/html/index.html

# Create a volume for persistent data
VOLUME /var/lib/mysql

# Switch to a non-root user if needed
USER www-data

# Expose ports
EXPOSE 80

# Define the default command when the container starts
CMD ["apache2ctl", "-D", "FOREGROUND"]
