# Use an Nginx base image
FROM nginx:alpine

# Remove the default nginx static files
RUN rm -rf /usr/share/nginx/html/*

# Copy static content to nginx serving directory
COPY ./react1 /usr/share/nginx/html

# Expose port 80 for the container
EXPOSE 80

# Start Nginx when the container has provisioned
CMD ["nginx", "-g", "daemon off;"]
