# Alpine Linux Node.js Docker Image

Alpine Linux: 3.4
Node.js: 6.2.0

## Use
```
FROM hafenio/node

COPY package.json /opt/package.json
RUN cd /opt; npm install
COPY . /opt
EXPOSE 3000
CMD [ "node", "/opt/src/index.js" ]
```
