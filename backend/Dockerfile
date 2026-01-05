FROM node:20-slim

WORKDIR /usr/src/app

COPY package*.json ./
RUN npm install

COPY . .

CMD ["sh", "-c", "npx prisma migrate deploy && npx prisma generate && node index.js"]
