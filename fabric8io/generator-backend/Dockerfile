FROM maven
RUN git clone https://github.com/fabric8io/generator-backend/
COPY pom.xml generator-backend/pom.xml
RUN cd generator-backend &&\
    mvn -B clean install

