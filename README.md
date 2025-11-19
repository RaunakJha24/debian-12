# Debian 12 “Bookworm” Installation Steps

## 1 Prepare for Installation
Download the Debian 12 “Bookworm” ISO from official [Debian website](https://www.debian.org/). Select the appropriate ISO for your computer. 
You can go for the full DVD version or netinst version of the ISO.

## 2 Audience & Scope

### 2.1 Who this is for
This guide is intended for system administrators or users familiar with basic system hardware BIOS/UEFI setup, who wish to install Debian 12.

### 2.2 What this covers
* Downloading and verifying Debain 12 installation media 
* Creating a bootable USB installation drive
* Booting the installer
* Basic installation: partitioning, user setup, software selection
* First-boot and initial configuration

## 3 Prerequisites

### 3.1 Hardware requirements(bare minimum)
For a typical desktop installations:
* Minimum 2GB RAM  
* At least 20 GB of storage
* UEFI firmware recommended; Secure Boot optional

### 3.2 Download media
* Visit the Debian download page and select the appropriate image for your architecture.
* Verify the download ISO’s checksum and optionally its GPG signature to ensure integrity. 

### 3.3 Bootable USB drive
* Prepare a USB disk (8GB or higher) to serve as installation media. 
* On Windows/Mac/Linux, Rufus/ Balena Etcher may be used.  

## 4 Installation Media
### 4.1 Create a Bootable USB Drive

Download and install Rufus or Balena Etcher according to your requirement and platform. 

### 4.2 Writing the ISO to USB

* Insert the USB stick (8 GB or larger).
* Open your chosen tool (Rufus, Balena Etcher)
* Select the downloaded ISO and choose the USB device as target.
* Start the write process and then eject the drive once the process is completed.

### 4.3 Verifying bootability

* Reboot your system and enter firmware (BIOS/UEFI) boot menu (typically by pressing F2/F10/Esc/F12).
* Select the USB drive.
* If you see the “Debian” installer menu, you are ready to proceed.

## 5 Installation Process

### 5.1 Start the Installer
* Choose the appropriate location and language.
* Choose the Keyboard layout.

### 5.2 Configuration
* The Installer will get you going once a network setting is detected. You may need to enter the password for the network profile.

### 5.3 Partitioning
Now, the option to select the mode of partitioning will show two options Manual or ***Use available free space***. Now, you will create two partitions: 
* Root(/): Select ext4 format and this is where Debian will be installed. 
* Swap: It is requred for a smoother performance. (You can select it as equivalent to the size of the RAM.)

### 5.4 Base System
Now, you need to install the base system. It will be done by the installer after it downloads the core packages.

### 5.5 Install the Bootloader (GRUB) 
The installer will prompt you to install the bootloader. You can do so by selecting the MBR of your main drive. 

### 5.6 User Account
Now, you need to select the User account and password for your system. 

### 5.7 Finish the process
* Finally you need to reboot the computer.
* You can eject the USB once you see the prompt on the screen.

## 6 Boot into Debian
* Now, the system the boot for the first time into Debian, you need to complete the process.
* Finally, you will be asked for the user password. 

