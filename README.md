# Basic - Project: Website Code | GitHub | Web Server - Hosting

This repository contains a step-by-step guide to set up and host a static website using Git and Mini-HTTPD on a Linux server. The process demonstrates how to clone your website code from GitHub and serve it through a simple HTTP server.

## Prerequisites
- A Linux-based virtual machine (VM) like an Ubuntu server.
- A public IP address for accessing the hosted website.
- Git installed on the server.

## Steps to Set Up the Server

1. **Update the Machine**
   ```bash
   sudo apt update -y
   ```

2. **Install Git**
   ```bash
   sudo apt install git -y
   ```

3. **Install Mini-HTTPD (Web Server)**
   ```bash
   sudo apt install mini-httpd -y
   ```

4. **Start and Enable Mini-HTTPD**
   ```bash
   sudo systemctl start mini-httpd
   sudo systemctl enable mini-httpd
   ```

5. **Navigate to the Web Root Directory**
   ```bash
   cd /var/www/html
   ```

6. **Clone the Website Repository**
   - Clone your website code from GitHub:
     ```bash
     git clone https://github.com/atulkamble/testwebsite.git
     ```
   - Alternatively, clone with `sudo` for permission issues:
     ```bash
     sudo git clone https://github.com/atulkamble/testwebsite.git
     ```

7. **Move Website Files to the Web Directory**
   ```bash
   sudo cp testwebsite/* .
   sudo mv testwebsite/css /var/www/html
   sudo mv testwebsite/js /var/www/html
   sudo mv testwebsite/images /var/www/html
   ```

8. **Access the Website**
   - Replace the public IP with your Azure VM's public IP and visit the website in your browser:
     ```
     http://<your-public-ip>/
     ```

   Example:
   ```
   http://98.70.89.130/
   ```

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

Let me know if you need any additional changes!
