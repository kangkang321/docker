FROM maven
RUN git clone https://github.com/fabric8io/generator-backend/ &&\
    mkdir -p /root/.m2/repository/org/jenkins-ci/jenkins/1.26
COPY pom.xml generator-backend/pom.xml
COPY jenkins-1.26.pom /root/.m2/repository/org/jenkins-ci/jenkins/1.26/jenkins-1.26.pom
RUN cd generator-backend &&\
    export MAVEN_OPTS=-Xms256m -Xmx2046m -XX:PermSize=128m -XX:MaxPermSize=256M &&\
    mvn -B clean install -Dmaven.test.skip=true

