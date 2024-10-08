# Use an official Node.js image
FROM node:16-alpine

# Set the working directory inside the container
WORKDIR /usr/src/app

# Copy the package.json and install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the port the app runs on
EXPOSE 8080

# Command to run the app
CMD ["node", "app.js"]
