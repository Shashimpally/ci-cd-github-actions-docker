# Use a smaller base image (optional, if you want smaller image)
FROM node:18-alpine

# Create app directory
WORKDIR /usr/src/app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install --production

# Copy only source files
COPY ./src ./src

# Expose port
EXPOSE 3000

# Start the app
CMD ["npm", "start"]
