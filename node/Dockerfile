FROM jboss/wildfly
ADD host-slave.xml /opt/jboss/wildfly/domain/configuration/host.xml
RUN /opt/jboss/wildfly/bin/add-user.sh admin admin --silent
CMD /opt/jboss/wildfly/bin/domain.sh -Djboss.domain.master.address=$MASTER_IP -b $NODE_IP -bprivate $NODE_IP