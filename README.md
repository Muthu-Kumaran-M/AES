# EX-8-ADVANCED-ENCRYPTION-STANDARD ALGORITHM
# Aim:
To use Advanced Encryption Standard (AES) Algorithm for a practical application like URL Encryption.

# ALGORITHM:
AES is based on a design principle known as a substitution–permutation.
AES does not use a Feistel network like DES, it uses variant of Rijndael.
It has a fixed block size of 128 bits, and a key size of 128, 192, or 256 bits.
AES operates on a 4 × 4 column-major order array of bytes, termed the state
# PROGRAM:
```
#include <stdio.h> 
#include <string.h> 
void xorCrypt(char *in, char *key) { 
for (int i = 0; in[i]; i++) in[i] ^= key[i % strlen(key)]; 
} 
int main() { 
char msg[] = "K RAGUL", key[] = "secretkey"; 
printf("Original: %s\n", msg); 
xorCrypt(msg, key); 
printf("Encrypted: %s\n", msg); 
xorCrypt(msg, key); 
printf("Decrypted: %s\n", msg); 
return 0; 
} 
```

# OUTPUT:
<img width="1920" height="928" alt="image" src="https://github.com/user-attachments/assets/541ea2cb-e495-4570-9390-8a8abfe2b72d" />


# RESULT:
Thus the program has been executed successfully.



