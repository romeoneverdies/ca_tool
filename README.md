# ca_tool
Self managed Local CA  tool


This is a quick script /Tool to create certificate more easily ... it uses openssl in backend. 

Edit the variables at the top to suit your own network/ca

the CA needs to be already setup its recomended you use a intermediate CA since you will be saving the password ( to sign the certs) 
so create a CA save that somewhere and add an intermediate that you can totogenerate the certs on the fly. 

this will generate csr, certificate key , validate those then it can create a ovpn from a template and append the certificates to it
the "view certificate" is defunct i think ( need some work) 

you need a openssl.cnf in the root of your Intermediate CA /CA
v3 extentions are usually required for servers and they are stored in the "EXTENSIONS" variable directory. 

Server certificates will be in the "certs" and the keys in "private" folders. 

User certifiates/key/files will be in their "certs/users/" and "private/users/" and "ovpn"  respective folders

there is also a pkcs12 conversion possible for both types of certificates...

compression flag to zip files to a web folder (local).. this is very usefull in my user portal project...


