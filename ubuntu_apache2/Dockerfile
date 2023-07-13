# Base image
FROM ubuntu:focal

# Install Apache2
RUN apt-get update 
	&& apt-get install -y apache2

# Copy Apache2 configuration
COPY ubuntu_apache2/apache2/sites-available/000-default.conf /etc/apache2/sites-available/000-default.conf

# Expose port 80
EXPOSE 80

# Start Apache2 service
CMD ["apachectl", "-D", "FOREGROUND"]
