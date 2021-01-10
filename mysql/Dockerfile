FROM mysql:5.7
LABEL OG=ztimage.com
COPY my.cnf /etc/mysql/conf.d/my.cnf
COPY ./ /temp/sql
RUN mv /temp/sql/*.sql /docker-entrypoint-initdb.d
RUN rm -rf /temp/sql
