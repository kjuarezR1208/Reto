FROM centos
RUN yum -y  install httpd 
RUN yum -y install php
RUN yum -y install git
RUN git clone  https://github.com/arcmop/retobase-nodejs.git
RUN cp -a /retobase-nodejs/* var/www/html
expose 80
CMD /usr/sbin/apache2ctl -D FOREGROUND
