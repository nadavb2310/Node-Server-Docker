# Set nginx base image
FROM nginx:latest

VOLUME /var/cache/nginx

# Copy custom configuration file from the current directory
COPY nginx.conf /etc/nginx/nginx.conf

EXPOSE 8080

#sets daemon off
RUN echo "daemon off;" >> /etc/nginx/nginx.conf

ENTRYPOINT [ "nginx" ]