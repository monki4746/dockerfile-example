From ubuntu:focal
ENV DEBIAN_FRONTEND-noninteractive
RUN apt-get update && apt-get install -y nginx
COPY nginx/sites-available/loadbalancer /etc/nginx/sites-available/loadbalancer
Run rm -f /etc/nginx/sites-enabled/default
Run ln -s /etc/nginx/sites-available/loadbalancer /etc/nginx/sites-enabled/loadbalancer
CMD ["nginx", "-g", "daemon off;"]
EXPOSE 80
