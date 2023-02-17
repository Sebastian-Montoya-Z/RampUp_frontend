FROM node:8.17
WORKDIR /usr/src/app
EXPOSE 8080
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run build
CMD ["sh", "-c", "npm start" ]