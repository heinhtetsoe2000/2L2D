FROM mysql:9.3.0

#COPY ./docker-entrypoint-initdb.d/ \
#    ./docker-entrypoint-initdb.d/

ARG MYSQL_USER
ARG MYSQL_PASSWORD

RUN { \
    echo "ALTER USER '${MYSQL_USER}'@'%' IDENTIFIED WITH mysql_native_password BY '${MYSQL_PASSWORD}';"; \
} > ./docker-entrypoint-initdb.d/user_init.sql