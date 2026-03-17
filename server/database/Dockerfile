FROM node:18.12.1-bullseye-slim

RUN npm install -g npm@9.1.3

WORKDIR /app

# Install dependencies
COPY package.json ./
RUN npm install

# Copy application source
COPY . .

EXPOSE 3030

CMD [ "node", "app.js" ]
