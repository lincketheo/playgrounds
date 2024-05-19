FROM nginx:1.25.1 
WORKDIR /app
COPY . .

COPY ./nginx.conf /etc/nginx/conf.d/nginx.conf
COPY ./www/ /usr/share/nginx/html
EXPOSE 8080
CMD ["nginx", "-g", "daemon off;"]
