# fixidia
a fix for Checkra1n after installing Sileo 

# Requirements:
* A PC with PuTTy (I don't know how to use it, so don't ask me) or a Mac.
* Download the zip file.
* Your Mac and iPhone should be connected to the same WiFi.
* (You can also do it on your iPhone via terminal, you can download terminus from App Store and SSH the device in port 44, IP 127.0.0.1)



Let's begin!



step 1:

Open Terminal and enter:

scp /path/to/fixidia.zip root@yourIPaddress:~/


replace /path/to/fixidia.zip with the actual path to it - you van also just drag the file onto the terminal.
replace yourIPaddress with your IP address found in the settings app.


step 2:

SSH into your iPhone as root.

(in terminal: "ssh root@yourIPaddress" without quotes.)


Step 3:

Enter the following commands one by one:

mkdir ~/APT

cd ~/APT

mv ../fixidia.zip .

chmod 777 fixidia.sh

./fixidia.sh




And you're done! The script will automatically delete itself and all of the resources used from your device.
