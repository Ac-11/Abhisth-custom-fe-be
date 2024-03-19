# Use an official Node runtime as the base image
FROM node:14

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the entire frontend directory to the container
COPY . .

# Expose port 3000 (assuming your frontend runs on port 3000)
EXPOSE 3000

# Command to run the React app
CMD ["npm", "start"]
