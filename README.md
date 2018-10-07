# A-comprehensive-guide-for-connecting-Raspberry-to-Laptop-Headless-Setup-
Use Laptop as a screen and its keyboard and mouse for Raspberry Pi computer


Follow step by step procedure to be successful:

1. First of all buy a SD card class 10 of 8-10 GB
2. Secondly download latest OS for Raspberry Pi from website. I recommend "Raspbian Stretch" Here is the link:
        https://www.raspberrypi.org/downloads/raspbian/
        
3. After downloading Plug in the SD card and format it using "SD card formatter" downloaded by website of sd-card-association
4. Write or burn all the files downloaded, by using Win32 Disk-Imager.
5. Now go to SD card (E: or G:) in your computer
6. Make two new empty files names as "ssh" and "wpa_supplicant.conf"
7. Open the "wpa_supplicant.conf" file and paste the following content in it: (Change SSID abd password according to your computer network)

ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
update_config=1
country=GB

network={
	ssid="Saad"
	psk="OMEPRAZOLE"
	key_mgmt=WPA-PSK

}


8. Plug in SD card and on the raspberry pi.
9. Now you've to download three softwares on the laptop. Putty, VNC viewer, IP scanner

Here are the three links:

https://www.advanced-ip-scanner.com/
https://www.realvnc.com/en/connect/download/vnc/windows/
https://www.putty.org/


10. Search IP address of pi using IP scanner.

11. Access the pi using putty and give it the IP address.
12. After successful login in the putty write:

sudo raspi-config

Go to ----> Advanced option and enable ---> VNC


13. Now open the VNC from your laptop
14. Enter the IP address

15.Check out the GUI Screen and enjoy using raspberry Pi.

For any queries and problems, you can ask me:

Syed Umaid Ahmed
+923323117626
syedumaidahmed96@gmail.com

for accessing the video tutorial, go to:

https://www.youtube.com/watch?v=E_xFFHvjtW0
