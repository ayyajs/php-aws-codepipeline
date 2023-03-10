sudo su  
sudo yum update -y

sudo yum install httpd -y  
yum install php72 php72-mysqlnd php72-imap php72-pecl-memcache php72-pecl-apcu php72-gd php72-mbstring -y

sudo yum install ruby -y  
sudo yum install wget -y  
cd /home/ec2-user  
wget https://aws-codedeploy-eu-central-1.s3.amazonaws.com/latest/install  
chmod +x ./install  
sudo ./install auto  
sudo service codedeploy-agent status  
service httpd start  
chkconfig httpd on
