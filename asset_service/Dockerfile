# FROM...
FROM node:17-alpine
# Create app directory
WORKDIR /app/src/app
# Install app dependencies
COPY package*.json ./
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
RUN npm install --only=production
# If you are building your code for production
# Bundle app source
COPY . .
EXPOSE 8008
CMD ["npm", "start"]