# Set nginx base image
FROM nginx:latest

VOLUME /var/cache/nginx

# Copy custom configuration file from the current directory
COPY nginx.conf /etc/nginx/nginx.conf

COPY ./public /var/www/public

EXPOSE 80 443

#sets daemon off
RUN echo "daemon off;" >> /etc/nginx/nginx.conf

ENTRYPOINT [ "nginx" ]