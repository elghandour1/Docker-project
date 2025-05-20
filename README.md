HTML + Nginx Docker Project

A minimal project to deploy a simple HTML file using Nginx inside Docker.

How to run

bash :
mkdir webseit
vim index.html
docker run -it -d --name html -p 8080:80 -v /home/ubuntu/website:/usr/share/nginx/html nginx 
