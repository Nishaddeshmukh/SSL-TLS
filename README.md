# SSL-TLS
This contains doc and information related to SSL/TLS


To understand working of ssl certificate follow this stackoverflow link :
https://stackoverflow.com/questions/188266/how-are-ssl-certificates-verified?rq=2



TLS :  

There are 3 vrsions of TLS protocol : TLS 1.1 , TLS 1.2 , TLS 1.3. The latest one is TLS1.3 and this is supported by new windows server machines 2022 and 2025 . windows 2019 will not support TLS .
So nowadays the commutnictaion on remote connections are happening using tls1.3 .  This is security protocol you can say which we will implement on top of existing sockets . If you have program where client is connecting to server using sockets then you can implement tls on top of that easily .

Next part and challenge is to select libraries orn supoorting package.  On linux systems you need not worry about package specifically rhel 8 and rhel9. This 2 systemwill have openssl no need to install separtly .
This openssl is having funcitons or api to use and build tls program . On winowds side we have schannel or sspi.h library for the same implementation.


