FROM mysql:8.0
ENV MYSQL_DATABASE=database
ENV MYSQL_USER=database
ENV MYSQL_PASSWORD=database
ENV MYSQL_ROOT_PASSWORD=database
#ADD ./dump/dump.sql /docker-entrypoint-initdb.d
COPY ./dump.sql /docker-entrypoint-initdb.d/dump.sql
RUN chmod 755 -R /var/lib/mysql
EXPOSE 3306:3306