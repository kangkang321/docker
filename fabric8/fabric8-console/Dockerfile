FROM node:6
RUN git clone https://github.com/kangkang321/fabric8-console && cd fabric8-console && npm install -g bower gulp && npm install && bower update --allow-root && mv -f k8s-proxy/hawtio-kubernetes.js libs/hawtio-kubernetes/dist/hawtio-kubernetes.js && mv -f k8s-proxy/hawtio-kubernetes-api.js libs/hawtio-kubernetes-api/dist/hawtio-kubernetes-api.js && gulp site && tar -czvf site.tar.gz site && mv site.tar.gz /root/ && cd .. && rm -rf fabric8-console
 
