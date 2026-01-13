# Backend Dockerfile
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package files
COPY apps/backend/src/package*.json ./

# Install dependencies
RUN npm ci

# Copy backend source code
COPY apps/backend/src/ ./

# Expose port
EXPOSE 3001

# Start the server
CMD ["npm", "start"]




