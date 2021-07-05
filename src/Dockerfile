FROM node:14.16.1-alpine3.13

LABEL Author="Ricardo Brandao"

#Set working directory from now on we will be inside /app
WORKDIR /app

#Copy packages files and install them
COPY package*.json ./
RUN npm install

#Copy the remaining items
COPY . .

EXPOSE 8080

CMD ["node", "app.js"]