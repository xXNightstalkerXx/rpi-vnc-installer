# rpi-kalivnc-installer
This Repository has some bash Scripts in it that download and setup the neccessary Files for the X11VNC Server on RPI Kali Linux.
The Installer creates a new Directory where this Repository get's downloaded into.

After downloading the necessary Files it will setup the VNC Server and ask you for a Password to secure your VNC Server.

The Installer also creates a backup of the /etc/init.d/vncserver and /home/kali/.vnc/xstartup Files before changing them!

I'm not an expert Coder so use this Repo on your own Risk and don't blame me if you have to reinstall your Raspberry.

If you find something interesting within my Scripts feel free to copy parts of it and implement it into your own code.
Also feel free to contribute to this Repository and make it better :)


----------------------------------------------------------------
----------------------------------------------------------------
# INSTALLATION

    wget https://raw.githubusercontent.com/xXNightstalkerXx/rpi-kalivnc-installer/master/rpi-kalivnc-installer
Download the Kalivnc Installer Script with wget

    sudo chmod 0755 rpi-kalivnc-installer
Make the file executable

    ./rpi-kalivnc-installer
Launch the Installer Script
</br>
</br>
The Installer does the rest of the Job for you now.

----------------------------------------------------------------
----------------------------------------------------------------
# HOW TO USE

    sudo systemctl start uctronics-lcd
Will start the uctronics-lcd service and activate the Status LCD until reboot

    sudo systemctl stop uctronics-lcd
Will stop the uctronics-lcd service and deactivate the Status LCD

    sudo systemctl enable uctronics-lcd
Enables the automatic startup of the Status LCD after boot

    sudo systemctl disable uctronics-lcd
Disables the automatic startup of the Status LCD after boot

    uctronics-lcd-uninstaller
Will revert all changes to /etc/modules, /boot/config.txt and systemd and switch off the I2C Interface.
Also delete's all associated Files.

----------------------------------------------------------------
----------------------------------------------------------------
