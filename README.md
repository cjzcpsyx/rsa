# rsa
A C program that implements "textbook" RSA encryption and decryption. Also includes the feature to generate RSA keys.
##Usage
1.Reads a public key K from the file key.oub, converts the string message to an integer m, and outputs the interger representation of E_k(m).
```
./rsa encrypt key.pub message
```
```
./rsa decrypt key.priv c
```
```
./rsa genkey numbits
```
