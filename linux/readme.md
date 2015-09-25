#Quick Ref for all things Linux

### How to check which versions of software is available for install
sudo apt-cache madison ^curl

Will show the versions of curl


### How to  redirect both stdout and stderr to same file
cmd >file.log 2>&1