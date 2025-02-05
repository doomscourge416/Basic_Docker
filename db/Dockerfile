FROM mysql:5.7.22

ARG MY_CNF_FILE

# Копируем пользовательский cnf

COPY ${MY_CNF_FILE} /etc/my.cnf

WORKDIR /var/lib/mysql

VOLUME /var/lib/mysql

CMD ["mysqld"]