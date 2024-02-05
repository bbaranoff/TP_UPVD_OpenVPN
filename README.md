# TP_UPVD_OpenVPN
Accès Réseau Linux

Installer VirtualBox

https://download.virtualbox.org/virtualbox/7.0.14/VirtualBox-7.0.14-161095-Win.exe

Installer l'extension pack

https://download.virtualbox.org/virtualbox/7.0.14/Oracle_VM_VirtualBox_Extension_Pack-7.0.14-161095.vbox-extpack

Télécharger Ubuntu 22.04

https://releases.ubuntu.com/22.04.3/ubuntu-22.04.3-desktop-amd64.iso


Début du TP instruction openvpn server uniquement

Sur une machine **virtuelle** Ubuntu 22.04 lancer

```bash
sudo apt update && sudo apt upgrade -y
sudo reboot
sudo apt install -y git python3-pip gcc make perl linux-headers-$(uname -r) texlive-xetex texlive-fonts-recommended texlive-plain-generic
wget http://download.virtualbox.org/virtualbox/7.0.14/VBoxGuestAdditions_7.0.14.iso
sudo mount -o loop VBoxGuestAdditions_7.0.14.iso /mnt
cd /mnt
sudo bash VBoxLinuxAdditions.run
reboot
pip3 install jupyterlab PyQtWebEngine
git clone https://github.com/bbaranoff/TP_UPVD_OpenVPN/
cd TP_UPVD_OpenVPN
jupyter lab
```
