FROM maven
RUN git clone https://github.com/fabric8io/generator-backend/ &&\
    git clone https://github.com/fabric8io/fabric8-generator/ &&\
    mkdir -p /root/.m2/repository/org/jenkins-ci/jenkins/1.26
COPY generator-backend.xml generator-backend/pom.xml
COPY fabric8-generator.xml fabric8-generator/pom.xml
COPY jenkins-1.26.pom /root/.m2/repository/org/jenkins-ci/jenkins/1.26/jenkins-1.26.pom
RUN cd fabric8-generator &&\
    mvn -B clean install -Dmaven.test.skip=true &&\
    cd ../generator-backend &&\
    mvn -B clean install -Dmaven.test.skip=true &&\
	cd .. &&\
	mv generator-backend/target/generator-swarm.jar generator-swarm.jar &&\
	rm -rf generator-backend &&\
	rm -rf fabric8-generator &&\
    rm -rf /root/.m2/repository	

