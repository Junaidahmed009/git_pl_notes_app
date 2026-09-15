FROM node:24

# creates a directory called /app in the container and sets it as the working directory
WORKDIR /app 

# copies package.json and package-lock.json to the working directory
COPY package*.json ./

# installs dependencies
RUN npm install

# copies the rest of the application code to the working directory
COPY . .

# exposes port 5173 for the application
EXPOSE 5173

# starts the application in development mode and binds it to all network interfaces
CMD ["npm", "run", "dev", "--", "--host"]