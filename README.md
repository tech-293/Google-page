# Google-page
Phishing-Page
Contents:

Introduction
Download
Starting the PHP server
Setting up the phishing site
Retrieving the credentials
Takeaways and awareness
Introduction
This project demonstrates how a hacker is able to easily create a deceptive phishing site by creating an HTML phishing page, using a PHP server to host the page, and using PHP code to retrieve the login credentials.

DISCLAIMER: This project was created for educational purposes only and is meant to raise awareness about the dangers of phishing emails and sites. This code and anything learned through this project should never be used on anyone without their consent.

Download
This project is avaliable for download in Kali Linux by entering the following commands in the terminal:

cd /home/kali
git clone https://github.com/jakeenea51/Phishing-Page
Starting the PHP server
This phishing site relies on a PHP server to host the HTML phishing page. The server will be running on port 8080. To start the server, enter the following commands:

cd /home/kali/Phishing-Page
bash server.sh
Setting up the phishing site
The link to get to the phishing site will be <ATTACKER'S IP>:8080/google.html

NOTE: This link will only work if you are connected to the same network as the victim.

Social engineering is the key to directing someone to the phishing site. The technique that is the most common is email. By creating an email that is convincing, the victim will be drawn to follow the link to the phishing page. Since the page I've created here is a fake Google account error page, I will create an email that makes the victim think there is an urgent error with their Google account and to fix it they must follow the link.

image

The link to the phishing page has been embedded in the word "link", so the victim won't know where they are being redirected unless they hover over the link.

image

After following the link, the victim will be redirected to the phishing page.

image

Retrieving the credentials
Once the credentials have been entered by the victim, they will be sent to a PHP script for handling and then outputted into a .txt file called "graveyard.txt" where the hacker can view all captured passwords.

image

image

Takeaways and awareness
This is just one very simple, yet effective, example of a phishing page that can be created to deceive people into entering their login credentials straight into a hacker's hands. Of course, to make the phishing site even more effective, the HTML code can be further developed to be even more convincing to the victim. Or in other cases, the source code of real login pages can be copied and changed so that the phishing page is a perfect replica of the real page, only differing in the fact that the credentials are being sent to the hacker instead of the desired recipient.

All this is to say that phishing sites are incredibly easy to create, meaning that it is important to always check the emails and links you receive before clicking on them. Here are a few things to always keep in mind to protect yourself from phishing attacks.

image
