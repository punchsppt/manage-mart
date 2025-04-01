# FROM node:16

# # WORKDIR /usr/src/app
# WORKDIR /app
# COPY package*.json ./
# RUN npm install
# COPY . .
# WORKDIR /app/src
# EXPOSE 3000
# # CMD ["npm", "start"]
# CMD [ "node", "app.js" ]
# Use Node.js as base image
FROM node:18

# Set working directory
WORKDIR /app

# Copy package files and install dependencies
COPY package.json package-lock.json ./
RUN npm install

# Copy entire backend source code (Make sure models/ is included)
COPY . .

# Expose port
EXPOSE 3000

# Start application
CMD ["node", "src/app.js"]
