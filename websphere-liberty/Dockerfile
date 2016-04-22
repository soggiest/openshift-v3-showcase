FROM websphere-liberty:webProfile6

USER 0

# Add binary deployment artifact to 'dropins' folder
#RUN wget --directory-prefix=/opt/ibm/wlp/usr/servers/defaultServer/dropins/ $BINARY_DEPLOYMENT_ARTIFACT_URL
COPY app/* /opt/ibm/wlp/usr/servers/defaultServer/dropins/

RUN chmod -Rf a+rw /bin;
RUN chmod -Rf a+rw /config;
RUN chmod -Rf a+rw /opt;
RUN chmod -Rf a+rw /etc;
RUN chmod -Rf a+rw /home;
RUN chmod -Rf a+rw /lib;
RUN chmod -Rf a+rw /lib64;
RUN chmod -Rf a+rw /dev;
RUN chmod -Rf a+rw /media;
RUN chmod -Rf a+rw /mnt;
RUN chmod -Rf a+rw /root;
RUN chmod -Rf a+rw /run;
RUN chmod -Rf a+rw /sbin;
RUN chmod -Rf a+rw /srv;
RUN chmod -Rf a+rw /tmp;
RUN chmod -Rf a+rw /usr;
RUN chmod -Rf a+rw /var;
RUN find / -type d -exec chmod a+x '{}' \;

# IBM WebSphere Liberty license must be accepted
ENV LICENSE $LICENSE
