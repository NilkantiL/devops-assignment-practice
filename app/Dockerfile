# 1. Use a Node.js base image
FROM node:18-alpine

# 2. Set the working directory inside the container
WORKDIR /app

# 3. Copy package.json and package-lock.json (if exists) to container
COPY package*.json ./

# 4. Install dependencies
RUN npm install

# 5. Copy the rest of your app code to the container
COPY . .

# 6. Specify the command to run your app
CMD ["npm", "start"]