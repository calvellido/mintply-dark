# Mintply-Dark

Dark version of Mintply, a Plymouth theme including a reimagined Linux Mint logo. Mintply is based on Edubuntu Plymouth. Linux Mint reimagined logo created by the same author of Mintply, <a href="http://tmoravec.cz" target="_blank">Tomáš Moravec</a>. The original Mintply theme can be found on <a href="http://linuxmint-art.org/content/show.php?content=159560" target="_blank">LinuxMint-Art</a>.

## Preview

![alt text](https://github.com/calvellido/mintply-dark/blob/master/mintply-dark.png "Mintply-Dark")


## Installation

Firt copy the `mintply-dark` directory over `/lib/plymouth/`, wou will need root privileges. Then install it on the system by the `update-alternatives` command:
```shell
sudo update-alternatives --install /lib/plymouth/themes/default.plymouth default.plymouth /lib/plymouth/themes/mintply-dark/mintply-dark.plymouth 100
```
Select the new installed theme to be the default by selecting its appropiate number:
```shell
sudo update-alternatives --config default.plymouth
```
And finally rebuild the image with:
```shell
sudo update-initramfs -u
```

Done, enjoy it!

[1]: http://tmoravec.cz
[2]: http://linuxmint-art.org/content/show.php?content=159560
