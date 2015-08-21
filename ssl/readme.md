#Quick Reference for all things SSL

### To debug SSL handshake issue with https server
openssl s_client -showcerts -connect localhost:8443


### To debug SSL handshake issue with https server and client authentication
openssl s_client -showcerts -connect localhost:8443 -key ibmclient.key -cert ibmclient.crt


