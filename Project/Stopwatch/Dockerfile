# Use a lightweight web server image. Nginx is a good choice.
FROM nginx:alpine

# Copy your static files into the Nginx default HTML directory.
COPY static /usr/share/nginx/html

# Expose port 80 (the default port for Nginx).
EXPOSE 80

# (Optional, but recommended) Healthcheck to ensure container is running
HEALTHCHECK --interval=5s --timeout=3s --retries=3 CMD ["curl", "-f", "http://localhost/"]

# (Optional) Add any other configuration or commands needed for your application.
# For example, you might want to customize the Nginx configuration.
# COPY nginx.conf /etc/nginx/conf.d/default.conf
