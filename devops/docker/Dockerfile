FROM node:18-alpine

WORKDIR /app

COPY package*.json ./

#RUN npm ci --only=production
RUN npm install --production

COPY . .

RUN mkdir -p images

EXPOSE 3000

CMD ["npm", "start"]