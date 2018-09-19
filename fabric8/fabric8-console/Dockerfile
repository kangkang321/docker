FROM node:6
RUN git clone https://github.com/kangkang321/fabric8-console && cd fabric8-console && npm install -g bower gulp && npm install && bower update --allow-root && gulp site && mv site /root/ && cd .. && rm -rf fabric8-console
 
