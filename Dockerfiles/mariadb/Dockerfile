# Set MariaDB base image
FROM mariadb:10.5

# File Author / Maintainer
MAINTAINER Toni Hermoso Pulido <toni.hermoso@crg.eu>

# Copy custom configuration file from the current directory
COPY mariadb-custom.cnf /etc/mysql/conf.d/custom.cnf

# Permissions
RUN usermod -u 1000 mysql; groupmod -g 1000 mysql
RUN chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 

# Volume
VOLUME /var/lib/mysql

# Define working directory.
WORKDIR /var/lib/mysql
