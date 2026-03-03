# Flask Local Network Web App

## Overview

This project is a simple web application built using the Flask framework in Python.
The main goal of this project is to understand how a local web server works and how a website running on a computer can be accessed from other devices on the same network.

The project demonstrates how backend web applications run locally and how devices such as phones can access the server through a private network.

---

# How It Works
When the Flask application runs, it starts a local development server on your computer.
Example:

http://127.0.0.1:5000

This address is called **localhost** and can only be accessed from the same computer.

To allow other devices to connect, the server runs on:

app.run(host="0.0.0.0", port=5000)

This allows the application to listen on the entire local network.

Example network access:

http://192.168.x.x:5000

Any device connected to the same WiFi network can open this address in a browser.

---

# Private Network Explanation

A private network is a local network created by a router.
Devices connected to the same WiFi receive private IP addresses like:

192.168.x.x
10.x.x.x
172.16.x.x – 172.31.x.x

These addresses are not accessible from the public internet.

Example structure:

Internet
➡️
Router
➡️
Local Devices
├Laptop (Flask Server)
- Phone
- Tablet

When the server runs on the laptop, the phone can access it using the laptop's local IP address.

---

# Project Features

• Python Flask backend
• Local development server
• Accessible from other devices on the same WiFi
• Demonstrates private network communication
• Simple structure for learning web development

---

# Project Structure

project-folder

app.py
templates/
static/
README.md

---

# How To Run The Project

1. Install Python
2. Install Flask

pip install flask

3. Run the server

python app.py

4. Open in browser

http://127.0.0.1:5000

or from another device on the network

http://YOUR-IP:5000

---

# Testing On Mobile

1. Connect phone to the same WiFi
2. Find your computer's IP address
3. Open it on the phone browser

Example:

http://192.168.1.37:5000

----

# Notes

This project uses Flask’s development server which is intended for learning and testing.
For production deployment a proper web server should be used.

---

# Learning Purpose

This project was created to understand:

• How web servers work
• How devices communicate in a local network
• Basics of backend web development
• Running and sharing a local website

---

# Author

Created as a learning project using Python and Flask.
