# Archefi86

Everything you need to install Arch Linux 64Bit in UEFI32.

## Dependencies 

git -> If you wish to clone the repo <br /> 
unzip -> If you want to download the Archefi86.zip and then unzip it. 

### Linux 
    
#### Arch LInux 
    sudo pacman -S git unzip 
    
#### Ubuntu 
    sudo apt install git unzip 
    
#### Debian 
    sudo apt-get install git unzip 
    
#### Windows 

WinRAR -> https://www.win-rar.com/download.html

#### MacOS 
Any Unzipping application (Good luck finding one that ain't a joke!)

## How to... 

You need a windows computer or any program that writes your arch ISO in 'ISO Mode' and not 'DD Mode' 

Then, 

#### Linux 
    lsblk 
    git clone --recursive 
    cd Archefi86/ 
    cp ./* /dev/sdX
    
Where, sdX is your USB drive. 

#### Windows 

You know the drill; copy everything in this repo to your (Arch Installer) USB drive. 

#### Mac OS
    diskutil list          
    git clone --recursive 
    cd Archefi86/ 
    cp ./* /dev/sdX
    
Where, sdX is your USB drive.

## Make sure to...

Open grub.cfg in your PC; To do so, type: 

Linux: vim ./boot/grub/grub.cfg <br /> 
Mac: Just dbl click on it while on finder! :) <br />  
Windows: notepad ./boot/grub/grub.cfg  

And replace 'USB-NAME' with the name of your USB stick as shown in your File Manager/Finder/This PC etc
If you used a program like rufus to flash your installation image then, the name of the USB stick should look something like ARCH_202207, or should atleast start with ARCH_2XXXXXX for the next 978 years. 

## Menu Entries 

As of today there are 'Arch specific' menuentries, and they are: (i) Intel, (ii) AMD and (iii) Universal 
Choose, Intel for intel CPUs, AMD for AMD Processors and Universal if you're not sure of your CPU
NB: This config only works on x86 or x86_64 systems with an Unified Extensible Firmware Interface (UEFI) 32Bits 
If you happen to have UEFI 64bit, you're in the wrong place; arch linux officaially supports you guys.

### HOW TO KNOW IF YOU HAVE EFI32!?
If your arch installer did'nt boot you into the live installation environment, then there is a high chance that you have an UEFI 32bit, in which case this repo should possibly fix it. 

## Problems? 
Just mail me at tedjoshissac@gmail.com

## Conclusion 
After copying the repository to your arch installer, just boot into it and select Universal or (a menu entry according to your CPU Manufacturer).
Enjoy! and Take it easy!
