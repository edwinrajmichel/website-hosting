Commands used :

Initially moving to the root user for permissions:
sudo su -

Then updating the packages:
yum update -y

Next installing Httpd service:
yum install -y httpd
systemctl status httpd

Next create a Directory:

mkdir demo
Move to the directory:
cd demo

Then paste the link copied in the github as a zip file
wget https://github.com/edwinrajmichel/website-hosting/archive/refs/heads/main.zip

Next Unzip the file:
unzip complex.zip
Then open the main directory 
cd complex
ls -lrt

Next move the contents to the /var/www/html:
mv * /var/www/html

Then enable the httpd service:
systemctl enable httpd
systemctl start httpd
systemctl status httpd
