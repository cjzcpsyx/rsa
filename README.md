# rsa
A C program that implements "textbook" RSA encryption and decryption. Also includes the feature to generate RSA keys.
##Usage
1.Reads a public key K from the file key.oub, converts the string message to an integer m, and outputs the interger representation of E(m).
```
./rsa encrypt key.pub message
```
2.Read a private key K from the file key.priv and putputs a string representation of the decryption D(c).
```
./rsa decrypt key.priv c
```
3.Outputs a private key(d, e, n), wherer n is approiamtely numbits bits long. You can store the key to a file using Uniex shell redirection:./rsa genkey 1024 > ky.priv
```
./rsa genkey numbits
```
##Sample outputs
```
$ ./rsa encrypt testkey.pub 'hello'
238301160525192269566546305624948574103

$ ./rsa decrypt testkey.priv 238301160525192269566546305624948574103
hello

$ ./rsa genkey 128
d 278503228302265047040587529645952279677
e 65537
n 288614444320069960785732511900748000413
```
