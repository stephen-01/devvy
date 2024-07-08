#!/bin/bash
sudo yum update -y
sudo yum install wget httpd -y
wget https://github.com/ceeepath/project-templates/archive/refs/tags/website_1.0.0.tar.gz
tar -xvf website_1.0.0.tar.gz
rm -rf website_1.0.0.tar.gz
cd project-templates-website_1.0.0/
tar -xvf template01.tar.gz
cd template01/
sudo mv index index.html
sudo cp -r * /var/www/html/
sudo chmod -R 755 /var/www/html
sudo systemctl enable httpd
sudo systemctl start httpd
sudo systemctl status httpd
