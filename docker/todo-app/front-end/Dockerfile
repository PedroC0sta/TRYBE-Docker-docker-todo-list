FROM node:14-alpine
COPY ./package.json .
RUN npm install
COPY . .
ADD node_modules.tar.gz .
EXPOSE 3000
WORKDIR /app

ENTRYPOINT [ "npm" ]
CMD [ "start" ]