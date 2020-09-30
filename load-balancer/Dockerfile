FROM jboss/wildfly
ADD host-slave.xml /opt/jboss/wildfly/domain/configuration/host.xml
RUN /opt/jboss/wildfly/bin/add-user.sh admin admin --silent
CMD /opt/jboss/wildfly/bin/domain.sh -Djboss.domain.master.address=192.168.1.10 -b 192.168.1.11 -bprivate 192.168.1.11