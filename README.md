# FileEncryptorAES-256
File encryption program written in C which uses the mbedtls library to perform AES-256 encryption on the given files.


```
./encrypt <mode> <input filename> <output filename> <key>
```

## IMPORTANT

_mode_ can be **any** permutation or substrings of the words _encrypt_ and _decrypt_ depending on what mode you want the program in.

e.g 
```
./encrypt eNcr filex filey key
```

## Usage

To begin with explode the mbedtls tarball.
```
tar xzvf mbedtls-2.6.0-apache.tgz
```

Build the mbedtls code.
```
cd mbedtls-2.6.0-apache.tgz
make
```

Go back up a level and compile the encryption program.
```
make
```

Run the encryption program
```
./encrypt
```

## Example

```
./encrypt encry input.txt cipher.bin decrypto

./encrypt dec cipher.bin recoveredplain.txt decrypto
```
