FROM node:16

# WORKDIR /usr/src/app
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
WORKDIR /app/src
EXPOSE 3000
# CMD ["npm", "start"]
CMD [ "node", "app.js" ]