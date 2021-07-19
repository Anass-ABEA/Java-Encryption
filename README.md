# RSA encryption
_Author:_ 
Anass **AIT BEN EL ARBI**
## Some Encryption methods used in Ciphers

 <ul>
     <li>AES/CBC/NoPadding (128)</li>
     <li>AES/CBC/PKCS5Padding (128)</li>
     <li>AES/ECB/NoPadding (128)</li>
     <li>AES/ECB/PKCS5Padding (128)</li>
     <li>RSA/ECB/PKCS1Padding (1024, 2048)</li>
     <li>RSA/ECB/OAEPWithSHA-1AndMGF1Padding (1024, 2048)</li>
     <li>RSA/ECB/OAEPWithSHA-256AndMGF1Padding (1024, 2048)</li>
 </ul>
 <p>
 for more details check out <a href="https://docs.oracle.com/javase/7/docs/api/javax/crypto/Cipher.html">Java Ciphers</a>


## Use of private and public key in a single application

class variables : 
```
private PrivateKey privateKey;
private PublicKey publicKey;
```
_____________
Encryption method: 
`
String encrypt(String message)
`
Uses `String encode(byte[])` to encode the encrypted message to a String
________
Decryption method:
`
String decrypt(String message)
`
Uses `String decode(byte[])` to decode the encrypted message to a String
________