### HTTPS POST with binary data
curl -k -X POST -H "Content-Type:application/octet-stream" https://localhost:8443/cxf/nsf/archive/filetransfer/ --data-binary "@path_to_my_file"

-k lets curl ignore the server name mismatch with name on the certificate


### HTTPS POST with 2-way SSL authentication
curl -k --cert ibmclient.crt --key ibmclient.key -X POST -H "Content-Type:application/octet-stream" https://localhost:8443/cxf/nsf/archive/filetransfer/ibmclient.pkcs12 --data-binary "@ibmclient.pkcs12"

