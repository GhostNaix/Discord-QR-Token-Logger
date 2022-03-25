# Discord-QR-Scam

### About
A Python script that automatically generates a Nitro scam QR code and grabs the Discord token when scanned. This tool demonstrates how people can trick others
into scanning their Discord login QR Code, and gain access to their account. Use for Educational Purposes only.

![img1](https://i.ibb.co/BL2Q0jz/Screenshot-527.png)

## Demonstration
![qr-code](https://user-images.githubusercontent.com/75003671/117522092-fd79ff80-afe3-11eb-938c-23dd68d5927c.gif)

## Usage
1. If you dont have python installed, download python 3.7.6
and make sure you click on the 'ADD TO PATH' option during
the installation.

2. Install the required modules > ```pip install -r requirements.txt``` or double click `pip_install_requirements.bat` also make sure to edit "URL" variable within the program to add your webhook!

3. Type ```python QR_Generator.py``` in cmd to run or double click `run_script.bat`

4. Wait for the `discord_gift.png` to be generated. Send the image to the victim and make them scan it.

5. QR Code only lasts about 2 minutes. Make sure you send a fresh one to the victim and he is ready to scan.

6. When the QR Code is scanned, you will automatically be logged in to their account and the script will grab the Discord token.

## Troubleshoot
Make sure your chromedriver.exe file is the same version as your current Chrome web browser version. To check your current Chrome version,
paste `chrome://settings/help` in Google Chrome.

if Chrome crashes,

1. Make sure your chromedriver.exe file is the same version as your Chrome web browser version
2. Download the latest version chromedriver.exe here: https://chromedriver.chromium.org/downloads
3. Then replace the chromedriver.exe file in the folder.

## Any Extra Help!

Join the Support Discord Server: https://discord.gg/a24Sp9bEXu 

## How it works
1. The python script opens a window into https://discord.com/login
2. The script converts the QR code on the website and downloads the image (contain a one time link that will allow login to a specfic request, from a specific browser, from a specfic IP address to log in), (The browser information, IP address, is not exposed in the QR code) - Correct me if I'm wrong
3. The script combines the QR code with the template
4. When the target scan the QR code logging in Discord will send data authenticating the browser in the QR which is the QR code in the template
5. The browser is refreshed on sucessful login and the token is extracted from the login the script detects this and logs it.
6. Done pretty much
7. (Optional) Sends it of the webhook of your choice
