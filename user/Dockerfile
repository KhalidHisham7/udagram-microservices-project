# Use NodeJS base image
FROM node:12

# Create app directory
WORKDIR /usr/src/app/user

# Install app dependencies by copying
# package.json and package-lock.json
COPY user/package*.json ./

# Install dependencies
RUN npm install

# Copy app source
COPY . .

# Bind the port that the image will run on
EXPOSE 8080

# Define the Docker image's behavior at runtime
CMD [ "npm", "run", "prod" ]