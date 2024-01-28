Basic - Project

Website Code | Github | Webser - Hosting
```
// updating machine
sudo apt update -y

// git install
sudo apt install git -y

// install httpd
sudo apt install mini-httpd -y

sudo systemctl start mini-httpd
sudo systemctl enable mini-httpd

cd /var/www/html

git clone https://github.com/atulkamble/testwebsite.git

sudo git clone https://github.com/atulkamble/testwebsite.git

sudo cp testwebsite/* .
sudo mv testwebsite/css /var/www/html
sudo mv testwebsite/js /var/www/html
sudo mv testwebsite/images /var/www/html

// Check public ip of your Azure VM (Replace Public ip)

http://98.70.89.130/

```
