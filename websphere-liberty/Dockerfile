FROM websphere-liberty:webProfile6

USER 0

# Add binary deployment artifact to 'dropins' folder
#RUN wget --directory-prefix=/opt/ibm/wlp/usr/servers/defaultServer/dropins/ $BINARY_DEPLOYMENT_ARTIFACT_URL
COPY app/* /opt/ibm/wlp/usr/servers/defaultServer/dropins/

RUN chmod -Rf a+rw /bin;
RUN find /bin -type d -exec chmod a+x '{}' \;
RUN chmod -Rf a+rw /config;
RUN find /config -type d -exec chmod a+x '{}' \;
RUN chmod -Rf a+rw /opt;
RUN find /opt -type d -exec chmod a+x '{}' \;
RUN chmod -Rf a+rw /etc;
RUN find /etc -type d -exec chmod a+x '{}' \;
RUN chmod -Rf a+rw /home;
RUN find /home -type d -exec chmod a+x '{}' \;
RUN chmod -Rf a+rw /lib;
RUN find /lib -type d -exec chmod a+x '{}' \;
RUN chmod -Rf a+rw /lib64;
RUN find /lib64 -type d -exec chmod a+x '{}' \;
RUN chmod -Rf a+rw /dev;
RUN find /dev -type d -exec chmod a+x '{}' \;
RUN chmod -Rf a+rw /media;
RUN find /media -type d -exec chmod a+x '{}' \;
RUN chmod -Rf a+rw /mnt;
RUN find /mnt -type d -exec chmod a+x '{}' \;
RUN chmod -Rf a+rw /root;
RUN find /root -type d -exec chmod a+x '{}' \;
RUN chmod -Rf a+rw /run;
RUN find /run -type d -exec chmod a+x '{}' \;
RUN chmod -Rf a+rw /sbin;
RUN find /sbin -type d -exec chmod a+x '{}' \;
RUN chmod -Rf a+rw /srv;
RUN find /srv -type d -exec chmod a+x '{}' \;
RUN chmod -Rf a+rw /tmp;
RUN find /tmp -type d -exec chmod a+x '{}' \;
RUN chmod -Rf a+rw /usr;
RUN find /usr -type d -exec chmod a+x '{}' \;
RUN chmod -Rf a+rw /var;
RUN find /var -type d -exec chmod a+x '{}' \;

# IBM WebSphere Liberty license must be accepted
ENV LICENSE $LICENSE
