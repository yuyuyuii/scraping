FROM mysql/mysql-server:8.0

ENV MYSQL_DATABASE=laravel \
  MYSQL_USER=my \
  MYSQL_PASSWORD=soad@090 \
  MYSQL_ROOT_PASSWORD=soad@090 \
  TZ=Asia/Tokyo

COPY ./my.cnf /etc/my.cnf
RUN chmod 644 /etc/my.cnf