# Use an official Node.js runtime as a parent image
FROM node:14-alpine

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the entire project directory to the container
COPY . .

# Build your React app
RUN npm run build

# Expose the port your React app runs on
EXPOSE 3000

# Command to run your app
CMD ["npm", "start"]
