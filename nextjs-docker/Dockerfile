# Install nodejs version 22
FROM node:22-alpine 

# Set working directory means (where the commands will be executed)
WORKDIR /app 

# Copy package.json and package-lock.json to working directory
COPY package*.json ./ 

# Install depedencies
RUN npm install

# Copy all files to working directory
COPY . . 

# Build the project
RUN npm run build

# Application access port, localhost:3000 or 127.0.0.1:3000 
EXPOSE 3000 

# Run the application
CMD ["npm", "start"] 