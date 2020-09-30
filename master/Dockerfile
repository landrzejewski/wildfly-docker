FROM jboss/wildfly
ADD domain.xml /opt/jboss/wildfly/domain/configuration/domain.xml
ADD host-master.xml /opt/jboss/wildfly/domain/configuration/host.xml
RUN /opt/jboss/wildfly/bin/add-user.sh admin admin --silent
CMD /opt/jboss/wildfly/bin/domain.sh -bmanagement 192.168.1.10
