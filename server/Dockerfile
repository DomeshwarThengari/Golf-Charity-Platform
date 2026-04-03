FROM node:20-alpine

WORKDIR /app

# Copy package files and install production dependencies
COPY package*.json ./
RUN npm install --production

# Copy server source code
COPY . .

# Expose port (adjust if your Express app defaults to something else)
EXPOSE 5000

# Start the Node server
CMD ["npm", "start"]
