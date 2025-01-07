# Use a Node.js base image
FROM node:16-alpine

# Set the working directory
WORKDIR /usr/src/app

# Copy the package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the front-end code into the container
COPY . .

# Expose the front-end server port
EXPOSE 3000

# Start the Next.js server
CMD ["npm", "run", "dev"]
