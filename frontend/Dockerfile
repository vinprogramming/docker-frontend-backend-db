# Stage 1: Build React app
FROM node:14 AS build
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
COPY .env.development .env
RUN npm run build

# Stage 2: Serve with Nginx
FROM nginx:alpine
COPY --from=build /app/build /usr/share/nginx/html
COPY nginx.conf /etc/nginx/conf.d/default.conf

# Expose ports and start Nginx
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
