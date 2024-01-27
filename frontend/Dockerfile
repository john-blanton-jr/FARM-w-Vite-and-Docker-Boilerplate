# Use the official Node.js 16 image.
FROM node:21-alpine

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install project dependencies
RUN npm install

# Copy the rest of your app's source code
COPY . .

# Build your app
RUN npm run build

# Start the app
CMD ["npm", "run", "dev"]
