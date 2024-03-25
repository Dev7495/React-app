# Installs node
FROM node:lts-alpine3.19

# Setting /react-app as working directory.
WORKDIR /react-app

# Copy package.json & package-lock.json to working dir.
COPY package*.json ./

# Installs dependencies - node_modules.
RUN npm install

# Copy all files to workdir.
COPY . .

# Exposing Port 3000 for app.
EXPOSE 3000

# Starts app.
CMD npm start