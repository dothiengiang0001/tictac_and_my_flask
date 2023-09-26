FROM node:18-alpine

RUN addgroup app && adduser -S -G app app
RUN mkdir /app && chown app:app /app
RUN chmod -R 777 /app

USER app
WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .

EXPOSE 5173

CMD ["npm", "run", "dev"]

