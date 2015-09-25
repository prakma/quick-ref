#Quick Ref for all things Linux

### How to check which versions of software is available for install
- sudo apt-cache madison ^curl
Will show the versions of curl

- sudo apt-get install vsftpd=2.3.5-3ubuntu1
will install a specific version

- sudo apt-cache pkgnames
will show all packages

- sudo apt-cache search gdb
will show the packagename and description. use it before installing

- sudo apt-cache show mysql
will show detail description of the package

- sudo apt-get remove vsftpd
will remove package without removing config files

- sudo apt-get purge vsftpd
will remove package AND their configuration files





### Add a new user
sudo adduser newuser

### Make an existing user sudo
sudo usermod -a -G sudo someuser

### Access VNC through SSH tunneling
Check this [link] (https://www.digitalocean.com/community/tutorials/how-to-install-and-configure-vnc-on-ubuntu-14-04)


### Forwarding from one port to another
- sudo iptables -t nat -I PREROUTING -p tcp --dport 443 -j REDIRECT --to-ports 8443
will forward the external facing 443 port to internal 8443 port.

- sudo iptables-save
will save the iptables rule changes

- sudo iptables -t nat -L -n -v
will show the current rules

### How to  redirect both stdout and stderr to same file
cmd >file.log 2>&1

