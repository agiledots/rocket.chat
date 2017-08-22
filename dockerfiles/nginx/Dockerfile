FROM nginx:latest
COPY ./nginx.conf /etc/nginx/nginx.conf
#RUN  openssl req -x509 -nodes -days 3650 -newkey rsa:2048 -subj "/CN=xxxx/O=xxxxx/C=JP" -keyout /etc/nginx/certificate.key -out /etc/nginx/certificate.crt
COPY ./certificate.key /etc/nginx/certificate.key
COPY ./certificate.crt /etc/nginx/certificate.crt

CMD  ["nginx", "-g", "daemon off;"]

