FROM node:6
RUN git clone https://github.com/kangkang321/fabric8-console && cd fabric8-console && npm install -g bower gulp && npm install && bower update --allow-root && gulp site && tar -czvf site.tar.gz site && mv site.tar.tz /root/ && cd .. && rm -rf fabric8-console
 
