FROM node:14-alpine
WORKDIR /app
COPY ./package.json .
RUN npm install
COPY . .
ADD node_modules.tar.gz .
EXPOSE 3000

ENTRYPOINT [ "npm" ]
CMD [ "start" ]