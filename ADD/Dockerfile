FROM almalinux:9
RUN dnf install nginx -y
RUN rm -f /usr/share/nginx/html/index.html
ADD https://raw.githubusercontent.com/nandagolla1/terraform-aws-instance/refs/heads/main/readme.MD /usr/share/nginx/html/index.html
RUN chmod +r /usr/share/nginx/html/index.html
CMD ["nginx", "-g", "daemon off;"]