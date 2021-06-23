## How https works

### Server Side
1. Generate public and private key
2. Send certificate sign request to CA with public key
3. CA sign certificate with CA private key, Anyone has the public key of CA can validate the request
4. Give signed certificate to server back

### Client side
1. Handshaking
    1. Client send request to server
    2. Server respond back with certificate and public key envrypted in it
    3. Client use the public key of CA to decrypt and get the public key of server
    4. With this client validates that request came from validate server
    5. Client encrypt client's public key using server public key and send it to server for secured communication after handshaking
2. Once keys are shared between client and server, all further communication will be done through encryption using shared key


![Image](https://github.com/impradeeparya/system-design/blob/main/https/https.png)
