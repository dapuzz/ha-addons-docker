FROM node:alpine

COPY . /
RUN apk update && apk upgrade && \
    apk add --no-cache bash git openssh
RUN cd /Baileys && npm update && npm i -f && cd .. && npm install -f

EXPOSE 8124
CMD [ "node", "index.js" ]
