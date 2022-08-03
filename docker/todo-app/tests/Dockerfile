FROM mjgargani/puppeteer:trybe1.0
COPY ./package.json .
RUN npm install
COPY . .
ADD node_modules.tar.gz .
WORKDIR /app

ENTRYPOINT [ "npm" ]
CMD [ "test" ]