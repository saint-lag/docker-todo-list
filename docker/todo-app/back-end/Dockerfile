FROM node:14-alpine AS todobackend
WORKDIR /app
COPY package*.json ./
RUN npm install
ADD node_modules.tar.gz ./
COPY . .
EXPOSE 3001
ENTRYPOINT ["npm", "start"]