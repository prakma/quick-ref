#Quick Reference for all things SSL

### To debug SSL handshake issue with https server
openssl s_client -showcerts -connect localhost:8443


### To debug SSL handshake issue with https server and client authentication
openssl s_client -showcerts -connect localhost:8443 -key ibmclient.key -cert ibmclient.crt


### To remove the password from the password protected pvt key file
openssl rsa -in <password protected .key file> -out <password_less_new_key_file.key>

Example with comments below:

For RSA keys, a suitable command for removing the passphrase would be:

openssl rsa -in /etc/ssl/private/example.key -out /etc/ssl/private/example.nocrypt.key

For DSA keys, replace rsa with dsa:

openssl dsa -in /etc/ssl/private/example.key -out /etc/ssl/private/example.nocrypt.key


