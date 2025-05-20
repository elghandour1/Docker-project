# HTML + Nginx Docker Project

A minimal project to deploy a simple HTML file using Nginx inside Docker.

## 🛠 How to Run

```bash
# Create directory and add HTML file
mkdir website
cd website
vim index.html

# Run Docker container
docker run -it -d --name html \
  -p 8080:80 \
  -v /home/ubuntu/website:/usr/share/nginx/html \
  nginx
