FROM node:8.17
WORKDIR /usr/src/app
EXPOSE 8080
COPY package*.json ./
COPY . .
RUN ls -la
RUN npm install
RUN npm run build
CMD PORT=8080 AUTH_API_ADDRESS=http://auth:8000 TODOS_API_ADDRESS=http://todos:8082 npm start