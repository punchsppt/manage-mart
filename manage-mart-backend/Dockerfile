FROM node:16

# WORKDIR /usr/src/app
WORKDIR /
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 3000
# CMD ["npm", "start"]
CMD [ "node", "app.js" ]