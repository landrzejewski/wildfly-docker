FROM jboss/wildfly
ADD host-slave.xml /opt/jboss/wildfly/domain/configuration/host.xml
RUN /opt/jboss/wildfly/bin/add-user.sh admin admin --silent
CMD /opt/jboss/wildfly/bin/domain.sh -Djboss.domain.master.address=master -b 0.0.0.0 -bprivate 0.0.0.0