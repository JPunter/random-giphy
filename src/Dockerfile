FROM nginx:1.19-alpine
RUN apk update && apk add curl
COPY . /usr/share/nginx/html
ADD startup.sh . 
RUN chmod +x startup.sh
EXPOSE 8080
CMD ["./startup.sh"]
