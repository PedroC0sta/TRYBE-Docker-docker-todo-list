FROM mjgargani/puppeteer:trybe1.0
WORKDIR /app
COPY ./package.json .
RUN npm install
COPY . .
ADD node_modules.tar.gz .

ENTRYPOINT [ "npm" ]
CMD [ "test" ]