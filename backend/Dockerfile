# Base image from Node.js official image
FROM node:16

# Create and set working directory inside container
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application
COPY . .

# Expose the port your app runs on (default for Node.js is 3000)
EXPOSE 3000

# Command to run your app
CMD ["node", "server.js"]
