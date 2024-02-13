# Wifi802.1xSkele
Skeleton code for connecting to a school wifi network on a system running NetworkManager (most linux distributions).

Name it "SSIDNAME".nmconnection , and fill out the information. The SSIDNAME will be the wifi you're connecting to.

Generate a UUID via the "uuidgen" command in the terminal.

Get interface information via the "ip address" command in the terminal.

Fill out the information, and move it to /etc/NetworkManager/system-connections/"SSIDNAME".nmconnection

Once done, connect to the wifi network using the "nmtui" terminal command.
