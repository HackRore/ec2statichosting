# ec2statichosting

Guide for learners to host a static web app on an EC2 instance of AWS.

## 🌐 EC2 Static Hosting Website

This repo contains a simple static website (`index.html`, `error.html`, and `style.css`) for hosting on an AWS EC2 Ubuntu instance using Apache2.

## 📁 Files

ec2statichosting/

├── index.html      # Homepage  
├── error.html      # Error page  
└── style.css       # CSS Styling

## 🚀 Deployment on EC2

### ✅ Prerequisites : 
- EC2 instance (Ubuntu)
- Apache2 & Git installed
- `.pem` SSH key

### 🔧 Steps

1. SSH into EC2 :
   
ssh -i "your-key.pem" ubuntu@your-ec2-public-ip

3. Install Apache & Git :
   
sudo apt update  
sudo apt install apache2 git -y

5. Go to Apache root :
   
cd /var/www/html

7. Remove default files
sudo rm -rf *

8. Clone this repo
sudo git clone https://github.com/HackRore/ec2statichosting.git .

9. Restart Apache
sudo systemctl restart apache2

## 🌍 Access Website

Visit:  
http://your-ec2-public-ip

✅ index.html loads homepage  
❌ Wrong paths show error.html

## 📺 Video Tutorial

Watch full step-by-step guide on YouTube:  
https://youtube.com/@CyberTechX_ravin

## 👨‍💻 Author

CyberTechX_ravin
🎓 B.E. (AI & DS)  
🔐 Cybersecurity & Cloud Enthusiast  
GitHub: https://github.com/HackRore  
YouTube: https://youtube.com/@CyberTechX_ravin
