# Start with a base image containing Java runtime
FROM nginx:latest

# Add Maintainer Info
LABEL maintainer="deleoney@globalhitss.com"

# Make port 81 available to the world outside this container
EXPOSE 81
COPY ./nginx/sites-enabled/locations.conf /etc/nginx/sites-enabled

# Copy the Angular applicatoin into the container
COPY ./dist/admin-otp /usr/share/nginx/html
