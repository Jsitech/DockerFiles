### Maligno Metasploit Payload Server
=====================================

***Maligno*** is an open source penetration testing tool written in Python that serves Metasploit payloads. It generates shellcode with msfvenom and transmits it over HTTP or HTTPS. The shellcode is encrypted with AES and encoded prior to transmission.

Maligno also comes with a client tool, which supports HTTP, HTTPS and encryption capabilities. The client is able to connect to Maligno in order to download an encrypted Metasploit payload. Once the shellcode is received, the client will decode it, decrypt it and inject it in the target machine.

The client-server communications can be configured in a way that allows you to simulate specific C&C communications or targeted attacks. In other words, the tool can be used as part of adversary replication engagements.


Maligno https://www.encripto.no/

***Quick Start***
=========================
```
docker run -i -t -p 443:443 2022:22 jsitech/maligno /bin/bash
```

***Share Directory for client file access***
=========================
```
docker run -i -t -p 443:443 -p 2022:22 -v /root/clients:/maligno-2.4/clients jsitech/maligno /bin/bash
```

***Maligno Configuration***
=========================
Configure Payloads, IP and port in server_config.xml
