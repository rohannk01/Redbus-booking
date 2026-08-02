FROM node:20

WORKDIR /app

# Copy everything
COPY . .

# Install frontend dependencies and build React
WORKDIR /app/frontend
RUN npm install
RUN npm run build

# Install backend dependencies
WORKDIR /app/Backend
RUN npm install

EXPOSE 3020

CMD ["npm", "start"]