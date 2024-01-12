# Use an official Node.js runtime as the base image
FROM node:16
# Set the working directory in the container
WORKDIR /app
# Copy package.json and package-lock.json to the working directory
COPY package*.json ./
# Install dependencies
RUN npm install
# Copy the application code to the container
COPY . .
# Expose port 8080
EXPOSE 5173:5173
# Start the application
CMD ["npm", "run", "dev", "--", "--host"]