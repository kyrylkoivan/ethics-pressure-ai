# web/Dockerfile

FROM node:20-slim

WORKDIR /app

# Copy dependency manifests
COPY package.json package-lock.json ./

# Install dependencies (this will pull the linux-x64-gnu lightningcss binary)
RUN npm install

# Copy application source
COPY . .

# Start in development mode
CMD ["npm", "run", "dev"]
