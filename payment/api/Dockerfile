FROM node:18

# Set the working directory inside the container
WORKDIR /app/payment/api

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install app dependencies
RUN npm install

# Copy the rest of the application code to the container
COPY . .

# Expose the port your app listens on
ENV PORT=${PORT:-3000}

# Define the command to start your Node.js app
CMD ["node", "server.js"]