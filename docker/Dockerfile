#install Tomcat 8.0.48 with JRE 8
FROM tomcat:8.0.48-jre8

RUN echo $CATALINA_HOME

RUN echo $JAVA_HOME

WORKDIR $CATALINA_HOME/tmp

#install HELM2 Web Service
ENV HELM2_WEBSERVICE_VERSION=3.0.5

RUN curl -o $CATALINA_HOME/webapps/WebService.war "https://oss.sonatype.org/service/local/repositories/releases/content/org/pistoiaalliance/helm/helm2-webservice/${HELM2_WEBSERVICE_VERSION}/helm2-webservice-${HELM2_WEBSERVICE_VERSION}.war"

#install HELM2 Monomer Service
ENV HELM2_MONOMERSERVICE_VERSION=1.1.11

RUN curl -o $CATALINA_HOME/webapps/HELM2MonomerService.war "https://oss.sonatype.org/service/local/repositories/releases/content/org/pistoiaalliance/helm/helm2-monomerservice/${HELM2_MONOMERSERVICE_VERSION}/helm2-monomerservice-${HELM2_MONOMERSERVICE_VERSION}.war"

#install HELM Web Editor
ENV HELM_WEB_EDITOR_VERSION=1.1.4

RUN curl -o $CATALINA_HOME/tmp/hwe.zip "https://github.com/PistoiaHELM/HELMWebEditor/releases/download/${HELM_WEB_EDITOR_VERSION}/hwe-${HELM_WEB_EDITOR_VERSION}.zip" -L

RUN unzip $CATALINA_HOME/tmp/hwe.zip

RUN cp -r $CATALINA_HOME/tmp/hwe $CATALINA_HOME/webapps

# copy index.html to ROOT folder to replace the default TOMCAT home page
COPY index.html $CATALINA_HOME/webapps/ROOT/index.html

#COPY tomcat-users.xml /usr/local/tomcat/conf

EXPOSE 8080

CMD ["catalina.sh", "run"]
