# Lab-9

## Task - 1

1) GitHub Actions allows us automate build tests and deployment pipeline.
2) I create file with name .github/workflows/github-actions-demo.yml and it creates new branch for this.
3) I check what create this file in Action tab.


## Task 2

1) docker save -o ubuntu_image.tar ubuntu:latest
Untagged: ubuntu:latest
Untagged: ubuntu@sha256:dfc10878be8d8fc9c61cbff33166cb1d1fe44391539243703c72766894fa834a
Deleted: sha256:b1e9cef3f2977f8bdd19eb9ae04f83b315f80fe4f5c5651fedf41482c12432f7

2) docker run -d -p 80:80 --name nginx_container nginx
Unable to find image 'nginx:latest' locally
latest: Pulling from library/nginx
a2318d6c47ec: Pull complete
095d327c79ae: Pull complete
bbfaa25db775: Pull complete
7bb6fb0cfb2b: Pull complete
0723edc10c17: Pull complete
24b3fdc4d1e3: Pull complete
3122471704d5: Pull complete
Digest: sha256:04ba374043ccd2fc5c593885c0eacddebabd5ca375f9323666f28dfd5a9710e3
Status: Downloaded newer image for nginx:latest
5aaea08f44c4bb59885d99cb78c3eea88b8efb1ed3de557e55a88f9bc0e9e37a
3) docker commit nginx_container my_website:latest

4) docker rm -f nginx_container
nginx_container
5) curl http://127.0.0.1:80
Give info from file index.html
6) docker diff my_website_container
C /etc
C /etc/nginx
C /etc/nginx/conf.d 
C /etc/nginx/conf.d/default.conf
C /run
C /run/nginx.pid