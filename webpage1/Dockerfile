FROM ubuntu:latest
# Update package list and install Apache
RUN apt-get update && apt-get install -y apache2 && apt-get clean

# Copy the web page to Apache's default directory
COPY index.html /var/www/html/index.html

# Expose port 80
EXPOSE 80

# Start Apache in the foreground
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]