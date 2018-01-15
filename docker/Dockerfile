#install Tomcat 8.0.48 with JRE 8
FROM tomcat:8.0.48-jre8

RUN echo $CATALINA_HOME

RUN echo $JAVA_HOME

WORKDIR $CATALINA_HOME/tmp

#install HELM2 Web Service
ENV HELM2_WEBSERVICE_VERSION=2.2.0

RUN curl -o $CATALINA_HOME/webapps/WebService.war "https://oss.sonatype.org/service/local/repositories/releases/content/org/pistoiaalliance/helm/helm2-webservice/${HELM2_WEBSERVICE_VERSION}/helm2-webservice-${HELM2_WEBSERVICE_VERSION}.war"

#install HELM2 Monomer Service
ENV HELM2_MONOMERSERVICE_VERSION=0.0.3

RUN curl -o $CATALINA_HOME/webapps/HELM2MonomerService.war "https://github.com/PistoiaHELM/HELMMonomerService/releases/download/${HELM2_MONOMERSERVICE_VERSION}/HELM2MonomerService.war" -L

#install HELM Web Editor
ENV HELM_WEB_EDITOR_VERSION=1.1.0

RUN curl -o $CATALINA_HOME/tmp/hwe.zip "https://github.com/PistoiaHELM/HELMWebEditor/releases/download/${HELM_WEB_EDITOR_VERSION}/hwe-${HELM_WEB_EDITOR_VERSION}.zip" -L

RUN unzip $CATALINA_HOME/tmp/hwe.zip

RUN cp -r $CATALINA_HOME/tmp/hwe $CATALINA_HOME/webapps

#COPY tomcat-users.xml /usr/local/tomcat/conf

EXPOSE 8080

CMD ["catalina.sh", "run"]
