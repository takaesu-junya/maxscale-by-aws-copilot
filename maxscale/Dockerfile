FROM mariadb/maxscale:6.3.1
RUN mv /etc/maxscale.cnf /etc/maxscale.cnf.bak && \
    cat /dev/null > /etc/maxscale.cnf
COPY mariadb.repo /etc/yum.repos.d/mariadb.repo
RUN yum update -y && \
    yum install mysql-client -y && \
    yum clean all
# RUN maxctrl create server aurora 192.168.0.221 3306

