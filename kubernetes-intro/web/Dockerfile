FROM nginx:1.25.3-alpine3.18-slim
RUN apk add --no-cache shadow
WORKDIR /app
RUN usermod -u 1001 nginx && groupmod -g 1001 nginx
COPY nginx.conf /etc/nginx/conf.d/default.conf
COPY homework.html .
EXPOSE 8000