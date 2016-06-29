# Alpine Linux Node.js Docker Image

Alpine Linux: 3.4

Node.js: 6.2.0

Size: 34.22 MB

## Node.js 6.2.0
#### Specs:
Alpine Linux: 3.4

Node.js: 6.2.0

Size: 34.22 MB
```
FROM hafenio/node

COPY package.json /opt/package.json
RUN cd /opt; npm install
COPY . /opt
EXPOSE 3000
CMD [ "node", "/opt/src/index.js" ]
```

## Node.js 6.2.2
#### Specs:
Alpine Linux: edge

Node.js: 6.2.2

Size: 32.55 MB
```
FROM hafenio/node:develop

COPY package.json /opt/package.json
RUN cd /opt; npm install
COPY . /opt
EXPOSE 3000
CMD [ "node", "/opt/src/index.js" ]
```
