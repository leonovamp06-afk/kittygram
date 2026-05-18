FROM node:18-alpine as build
WORKDIR /app
# В реальном проекте здесь будет сборка фронтенда
RUN echo "Frontend placeholder" > /app/index.html
FROM nginx:1.22
COPY --from=build /app/index.html /usr/share/nginx/html/index.html