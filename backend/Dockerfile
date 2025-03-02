#FROM node:20
#for optimize docker take alpine version base OS
FROM node:20.18.3-alpine3.21
WORKDIR /opt/backend
COPY package.json .
COPY *.js .
RUN npm install
#LOcal host fro host network
#ENV DB_HOST="localhost"
ENV DB_HOST="mysql"
CMD ["node", "index.js"]