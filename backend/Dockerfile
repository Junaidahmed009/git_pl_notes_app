FROM node:24

# creates a directory called /app in the container and sets it as the working directory
WORKDIR /app 

# copies package.json and package-lock.json to the working directory
COPY package*.json ./

# installs dependencies
RUN npm install

# copies the rest of the application code to the working directory
COPY . .

# exposes port 3000 for the application
EXPOSE 3000

CMD ["npm", "start"]