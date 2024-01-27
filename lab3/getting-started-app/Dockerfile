# Source Image (usually an Operating System)
FROM node:18-alpine

# Directory where files are stored inside our container
WORKDIR /app

# Command to copy files from our local folder on..
# ..local machine to local folder in the container
COPY . .

# Running the build command of the yarn build tool
RUN yarn install --production

# Executing a terminal command to run a node server
CMD ["node", "src/index.js"]

# Exposing our image port so outside images can attach to it
EXPOSE 3000