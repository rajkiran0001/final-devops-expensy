# Stage 1: Build
FROM node:18-alpine AS builder

WORKDIR /app

COPY . .

# Install dependencies
RUN npm install

# Build TypeScript
RUN npm run build
# Stage 2: Run

# Expose app port
EXPOSE 8706
# Start the backend
CMD ["node", "dist/server.js"]