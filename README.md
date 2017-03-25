# AES
C++ AES(Advanced Encryption Standard) implementation

**This class is very simple to use:**
```c++
...


unsigned char plain[] = { 0x00, 0x11, 0x22, 0x33, 0x44, 0x55, 0x66, 0x77, 0x88, 0x99, 0xaa, 0xbb, 0xcc, 0xdd, 0xee, 0xff }; //plaintext example
unsigned char key[] = { 0x00, 0x01, 0x02, 0x03, 0x04, 0x05, 0x06, 0x07, 0x08, 0x09, 0x0a, 0x0b, 0x0c, 0x0d, 0x0e, 0x0f }; //key eaxmple
unsigned int plainLen = 16 * sizeof(unsigned char);  //bytes in plaintext
unsigned int outLen = 0;  // out param - bytes in сiphertext

AES aes(128);  //128 - key length, can be 128, 192 or 256
out = aes.EncryptECB(plain, plainLen, key, outLen);
//now out contains outLen bytes - ciphertext
...
```
ECB, CBC, CFB modes are supported.


For more tests and examples see [Main file](https://github.com/SergeyBel/AES/blob/master/main.cpp)

You can read more about AES here:

https://en.wikipedia.org/wiki/Advanced_Encryption_Standard

http://nvlpubs.nist.gov/nistpubs/FIPS/NIST.FIPS.197.pdf


