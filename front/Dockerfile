# Use an official Node.js runtime as a parent image
FROM node:18-alpine

# Set the working directory to /app
WORKDIR /app

# Copy the package.json and package-lock.json files to the container
COPY package*.json ./

# Install the app's dependencies
RUN npm install

# Copy the rest of the app's files to the container
COPY . .

# Build the app
RUN npm run build

EXPOSE 8081

# Set the command to run when the container starts
CMD ["npm", "start"]
