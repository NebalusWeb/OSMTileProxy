FROM nginx:stable-alpine AS base
COPY ./docker/nginx/default.conf /etc/nginx/conf.d/default.conf
RUN mkdir -p /var/cache/nginx/tiles && chown -R nginx:nginx /var/cache/nginx/tiles
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]