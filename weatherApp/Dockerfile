FROM node:alpine

WORKDIR /app

COPY package.json .

COPY package-lock.json .

RUN npm install

COPY . .

RUN npm run build

#####

FROM nginx

WORKDIR /usr/share/nginx/html

COPY --from=0 /app/dist .

EXPOSE 80
