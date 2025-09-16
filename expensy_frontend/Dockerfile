# Step 1: Use an official Node.js image as the base image
FROM node:18-alpine

# Step 2: Set the working directory in the container
WORKDIR /app

# Step 5: Copy the rest of the application code
COPY . .

# Step 4: Install the dependencies
RUN npm install


# Step 6: Build the Next.js app (production build)
RUN npm run build

# Step 7: Expose the port that Next.js will run on
EXPOSE 3002

# Step 8: Start the Next.js app
CMD ["npm", "start"]