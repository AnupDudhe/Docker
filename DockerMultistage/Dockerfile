# Base stage: Install dependencies
FROM node:18 AS base

WORKDIR /app
COPY package*.json ./

# Development stage
FROM base AS development

RUN npm install
COPY . .
# Install nodemon globally for hot reloading
RUN npm install -g nodemon

CMD ["nodemon", "src/index.js"]

# Production stage
FROM base AS production

# Install only production dependencies
RUN npm install --only=production
COPY . .

# Start the app
CMD ["node", "src/index.js"]
