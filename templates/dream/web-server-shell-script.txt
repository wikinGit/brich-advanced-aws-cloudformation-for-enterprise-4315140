#!/bin/bash
#User data for new EC2 instances
#install httpd (Linux 2 version)
sudo yum update - y
sudo yum install - y httpd
sudo systemctl start httpd
sudo systemctl enable httpd
echo "<h1>Daydreams Travel Agency! This is $(hostname -f)</h1>"
/var/www/html/index.html