FROM postgres:17-alpine

WORKDIR /var/lib/postgresql/data

COPY init.sql /docker-entrypoint-initdb.d/

EXPOSE 5432