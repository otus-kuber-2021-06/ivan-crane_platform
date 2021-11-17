FROM nginx:1.20.2-alpine
EXPOSE 8000
COPY /index.html /app/
COPY config /etc/nginx/conf.d/default.conf
CMD ["nginx","-g","daemon off;"]
