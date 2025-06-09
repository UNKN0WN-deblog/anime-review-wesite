# Anime Review Website 🎌✨

This is my ICT171 Assignment 2 cloud deployment project for Murdoch University. The project demonstrates the setup and deployment of a static anime review website on an AWS EC2 instance using Apache2. It showcases spoiler-free reviews of popular anime titles using HTML, CSS, and cloud infrastructure, with future support for backend features and user interaction.

---

## 🌐 Live Website

Visit the deployed site at:  
🔗 [http://daifu.click](http://daifu.click)  
🔐 [https://daifu.click](https://daifu.click) *(SSL enabled with Let’s Encrypt)*

---

## 🎓 Student Information

- 👤 Name: Roshan shrestha  
- 🆔 Student ID: 35318397  
- 📚 Unit: ICT171 – Introduction to Server Environments and Architectures  
- 🖥 Project Title: Anime Review Website  
- 🗓 Year: 2025  
- 🌐 Domain: daifu.click  
- ☁ Hosting: Amazon EC2 (Ubuntu + Apache2)

---

## 📁 Project Contents

This repository contains:

- `index.html` – main webpage with anime summaries
- `styles.css` – website styling and layout
- `images/` – anime logos and thumbnails
- `LICENSE_CODE.txt` – MIT License for code
- `LICENSE_CONTENT.txt` – Creative Commons license for content
- `README.md` – this documentation

---

## ⚙ Technologies Used

- Amazon EC2 (Ubuntu 22.04 LTS)
- Apache2 Web Server
- SCP (Secure Copy) for file uploads
- Certbot (Let’s Encrypt SSL setup)
- SSH terminal for deployment
- HTML5 & CSS3 (static site)

---

## 🖼 Image Attribution

All anime logos (e.g. AOT, Demon Slayer, One Piece) are sourced from **public domain** or **official logo assets** and are used only for educational purposes.  
No copyright infringement is intended.

---
## video explainer: 
https://youtu.be/UqIX3bnoirA?si=FAf51T78pqwcw6ye 

## 🛡 Licenses

- **Code** licensed under the [MIT License](LICENSE_CODE.txt)
- **Content** licensed under the [Creative Commons Attribution 4.0 International License](LICENSE_CONTENT.txt)

> 🔒 All visual assets are excluded from these licenses and are not for redistribution.

---

## 📂 How to Clone & Deploy

1. Clone this repo:
   ```bash
   git clone https://github.com/your-username/anime-review-website.git
   cd anime-review-website
   ```

2. Upload to EC2 and deploy using:
   ```bash
   scp -i "Anime.pem" anime-review-website.zip ubuntu@your-ec2-ip:~
   ssh -i "Anime.pem" ubuntu@your-ec2-ip
   unzip anime-review-website.zip -d anime-site
   sudo cp anime-site/* /var/www/html/
   sudo chown -R www-data:www-data /var/www/html
   sudo chmod -R 755 /var/www/html
   ```

3. Enable HTTPS:
   ```bash
   sudo apt install certbot python3-certbot-apache -y
   sudo certbot --apache -d daifu.click -d www.daifu.click
   ```

---

## ✅ Future Enhancements

- Dynamic backend using Node.js or PHP
- User login and comment system
- Anime filter by genre/year
- Review submission via web form
- REST API for content delivery

---

## 📬 Contact

Have suggestions or want to contribute?  
Open an issue or fork the repo and submit a pull request.
