FROM nginx
WORKDIR /app
RUN chown -R 1001:1001 /app && chmod -R 755 /app && \
        chown -R 1001:1001 /var/cache/nginx && \
        chown -R 1001:1001 /var/log/nginx && \
        chown -R 1001:1001 /etc/nginx/conf.d
RUN touch /var/run/nginx.pid && \
        chown -R 1001:1001 /var/run/nginx.pid
COPY nginx.conf /etc/nginx/nginx.conf
USER 1001
COPY *.html .
COPY example.conf /etc/nginx/conf.d/
