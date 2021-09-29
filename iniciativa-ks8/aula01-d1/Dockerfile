FROM node:14.17
WORKDIR /app
COPY conversao-temperatura/src/package*.json ./
RUN npm install
COPY conversao-temperatura/src/ .
EXPOSE 5000
CMD ["node", "server.js"]