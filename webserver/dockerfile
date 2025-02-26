# Gebruik het officiële NGINX image van Docker Hub
FROM nginx:stable-alpine

# Kopieer de website-inhoud naar de container
#COPY ./html/index.html /usr/share/nginx/html/index.html
COPY webserver/html/index.html /usr/share/nginx/html/index.html

# Stel de container bloot aan poort 80
EXPOSE 80

# Start NGINX
CMD ["nginx", "-g", "daemon off;"]