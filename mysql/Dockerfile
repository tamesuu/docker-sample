FROM mysql:5.6

ARG my_cnf
RUN chmod 777 /var/log/mysql

COPY $my_cnf /etc/mysql/conf.d/my.cnf
