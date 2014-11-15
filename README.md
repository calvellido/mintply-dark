mintply-dark
============

Dark version of Mintply, a Plymouth theme including a reimagined Linux Mint logo.
Mintply is based on Edubuntu Plymouth. 
Linux Mint reimagined logo created by the same author of Mintply, Tomáš Moravec (http://tmoravec.cz).
The original Mintply can be found on: http://linuxmint-art.org/content/show.php?content=159560

Installation.
============

#sudo update-alternatives --install /lib/plymouth/themes/default.plymouth default.plymouth /lib/plymouth/themes/mintply-dark/mintply-dark.plymouth 100

#sudo update-alternatives --config default.plymouth

Finally rebuild the image with
#sudo update-initramfs -u
