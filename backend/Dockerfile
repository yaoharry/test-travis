FROM node:12-alpine

# avoid running app as root
RUN mkdir -p /home/node/app/node_modules && chown -R node:node /home/node/app

WORKDIR /home/node/app

COPY package*.json ./

# switch from root
USER node

RUN npm install

COPY --chown=node:node . .

EXPOSE 3000
EXPOSE 8000
EXPOSE 27017

CMD [ "npm", "start" ]

