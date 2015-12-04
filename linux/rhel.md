## Red Hat Enterprise Linux Frequently used Commands

### How to install a extract and install a specific file from .rpm
- rpm -qlp httpd-2.0.40-21.i386.rpm | grep htpasswd
will query the rpm  for htpasswd file and show the location where it will be installed

- rpm2cpio php-5.1.4-1.esp1.x86_64.rpm | cpio -idmv
Will extract files from rpm and put it in the current directory

- rpm2cpio httpd-2.0.40-21.i386.rpm | cpio -ivd ./usr/bin/htpasswd
will extract a single htpasswd file and put it in the current directory

- sudo yum install /tmp/usr/lib64/libavformat.so.54
Will install this file from the curent /tmp/* location

