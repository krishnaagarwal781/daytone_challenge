# Use official Node.js image as a parent image
FROM node:18-alpine

# Set the working directory inside the container
WORKDIR /workspace

# Copy the package.json and package-lock.json
COPY ./frontend/package*.json /workspace/

# Install dependencies
RUN npm install

# Copy the rest of the frontend code
COPY ./frontend /workspace/

# Expose port 3000 for Next.js
EXPOSE 3000

# Run the Next.js development server
CMD ["npm", "run", "dev"]
