#Quick Ref for all things Linux

### How to check which versions of software is available for install
sudo apt-cache madison ^curl

Will show the versions of curl


### Add a new user
sudo adduser newuser

### Make an existing user sudo
sudo usermod -a -G sudo someuser

### Access VNC through SSH tunneling
Check this [link] (https://www.digitalocean.com/community/tutorials/how-to-install-and-configure-vnc-on-ubuntu-14-04)