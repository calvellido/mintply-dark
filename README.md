# Mintply-Dark

Dark version of Mintply, a Plymouth theme including a reimagined Linux Mint logo. Mintply is based on Edubuntu Plymouth. Linux Mint reimagined logo created by the same author of Mintply, <a href="http://tmoravec.cz" target="_blank">Tomáš Moravec</a>. The original Mintply theme can be found on <a href="http://linuxmint-art.org/content/show.php?content=159560" target="_blank">LinuxMint-Art</a>.

## Preview

![alt text](https://github.com/calvellido/mintply-dark/blob/master/mintply-dark.png "Mintply-Dark")


## Installation

```shell
git clone https://github.com/calvellido/mintply-dark.git
```

First copy the `mintply-dark` directory over `/lib/plymouth/themes/` or `/usr/share/plymouth/themes/` depending on where your Plymouth installation sits, wou will need root privileges for this. Check that the directory set on ![mintply-dark/mintply-dark.plymouth](https://github.com/calvellido/mintply-dark/blob/master/mintply-dark/mintply-dark.plymouth "mintply-dark/mintply-dark.plymouth") file is correct.

```shell
cp -r mintply-dark/mintply-dark /usr/share/plymouth/themes/
```

Then install the theme on the system by the `update-alternatives` command:
```shell
sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/mintply-dark/mintply-dark.plymouth 100
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
