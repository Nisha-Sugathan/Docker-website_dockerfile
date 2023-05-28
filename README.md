# Docker-website_dockerfile
Dockerfile is a script to build docker image . A Dockerfile is a text document that contains all the commands a user could call on the command line to assemble an image. Docker can build images automatically by reading the instructions from a Dockerfile


### Prerequisites
Need to install docker on your machine
Add your username to docker group

### Docker Installation

```
sudo yum install docker -y &> /dev/null
sudo systemctl restart docker.service
sudo systemctl enable docker.service
sudo usermod -a -G docker ec2-user
```
![docker_installation](https://github.com/Nisha-Sugathan/Docker-Bind_mounting/assets/134600837/ba7797c4-9a73-4ce6-b593-2befa5850e0d)

### copy a site template to public_html and modify httpd.conf DirectoryIndex
```
wget https://www.tooplate.com/zip-templates/2133_moso_interior.zip
unzip 2133_moso_interior.zip
cp -r 2133_moso_interior/* public_html/
ls -al public_html/
```
Screenshot of current site files


![site_files](https://github.com/Nisha-Sugathan/Docker-website_dockerfile/assets/134600837/47b0928c-fc86-4ae6-a7a9-5f589c8e5efb)
