#!/bin/bash

cd ~
sudo yum install -y nginx
sudo systemctl start nginx
sudo systemctl enable nginx
sudo git clone https://github.com/ChinenyenwaN1/ACS-project-configuration.git
sudo cp /ACS-project-configuration/reverse.conf /etc/nginx/
sudo mv /etc/nginx/nginx.conf /etc/nginx/nginx.conf-distro
cd /etc/nginx/
sudo touch nginx.conf
sudo sed -n 'w nginx.conf' reverse.conf
sudo systemctl restart nginx
sudo rm -rf reverse.conf
sudo rm -rf /ACS-project-configuration



