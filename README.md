# Wifi802.1xSkele
Skeleton code for connecting to an 802.1x school wifi network on a system running NetworkManager (most linux distributions).

# Instructions
1.) **Download** the enterpriseSkeleton.txt file in this repo.

2.) **Name it** `"SSIDNAME".nmconnection`  , and fill out the information inside it. The SSIDNAME will be the wifi you're connecting to.

3.) **Generate a UUID** via the  `uuidgen`  command in the terminal, add it to the UUID line in the file.

4.) **Get interface information** via the `ip address`  command in the terminal. add it to the interface-name line in the file.



5.) **Fill out the rest of the information** (username, password, SSID name) and **move it** to:

/etc/NetworkManager/system-connections/"SSIDNAME".nmconnection via

`mv $(pwd)/"SSIDNAME".nmconnection /etc/NetworkManager/system-connections/"SSIDNAME".connection` 


6.) **Set the correct permissions** on the file with: 

`sudo chown root:root /etc/NetworkManager/system-connections/"SSIDNAME".nmconnection` 

`sudo chmod 600 /etc/NetworkManager/system-connections/"SSIDNAME".nmconnection` 

# Connect

Once done, connect to the wifi network using the `nmtui`  terminal command.
