# Use the official Node.js image as the base image
FROM node:18

# Set the working directory inside the container
WORKDIR /app/SCD_Q1_Comments

# Set environment variables
ENV NODE_ENV=production
ENV PORT=3000

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code to the working directory
COPY . .

# Expose the port the app runs on
EXPOSE 3000

# Define the command to run the application
CMD ["npm", "start"]