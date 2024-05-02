# Dell PowerEdge R720 Server Setup

This guide provides instructions on how to set up RAID on a Dell PowerEdge R720 server, install Ubuntu Server, and connect to the machine using SSH.

## Setting Up RAID

1. **Boot the server**: Start the Dell PowerEdge R720 server.
2. **Enter the Virtual Disk Manager (VDM)**: During the booting process, press `CTRL + R` to enter the VDM.
3. **Create a Virtual Disk**: In the VDM, create a new Virtual Disk.
4. **Add Physical Disks**: Add the physical disks to the Virtual Disk you just created.
5. **Specify the RAID Version**: Choose the appropriate RAID version for your setup.
6. **Save and Exit**: Save the configuration and exit the VDM.
7. **Reboot the Server**: Restart the server for the changes to take effect.

For a visual guide on how to perform these steps, refer to this video tutorial.
[IP Core Networks](https://www.youtube.com/watch?app=desktop&v=w0OzH9Rk08g)

## Installing Ubuntu Server

1. **Enter the BIOS**: During the reboot, enter the server's BIOS.
2. **Enable UEFI**: In the BIOS, enable the UEFI boot mode.
3. **Boot from OS Installer**: Choose to boot from the device that contains the Ubuntu Server installer.
4. **Install Ubuntu Server**: Follow the prompts to install Ubuntu Server on your machine.

If you encounter any issues during the installation, this guide may be helpful.
[TechHut](https://www.youtube.com/watch?v=K2m52F0S2w8)

## Setting Up and Connecting via SSH

To set up SSH on the server and connect to it, refer to the "SSH service" section under "Networking" in the "Basics of Linux system" of my guide.
[SSN repo](https://github.com/nerdpai/Sieczka-Systems-Networking/blob/main/Systems.md)
