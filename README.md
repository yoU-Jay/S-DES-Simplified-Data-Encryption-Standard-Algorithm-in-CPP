# S-DES-Simplified-Data-Encryption-Standard-Algorithm-in-CPP
Simplified Data Encryption Standard (S-DES) is a simple version of the DES Algorithm. It is similar to the DES algorithm but is a smaller algorithm and has fewer parameters than DES. It was made for educational purposes so that understanding DES would become simpler.
### Sample Output
```
Enter 10-bit Master Key (using space)
1 0 0 1 0 0 0 0 0 1 0

KEY GENERATION..

After P10 Permutation: 1 0 0 0 0 0 1 1 0 0 

After split, 
l = 1 0 0 0 0 
r = 0 1 1 0 0 

After LeftShift-1, 
l = 0 0 0 0 1 
r = 1 1 0 0 0 

After P8, Key-1: 1 0 1 0 0 1 0 0 

After LeftShift-2, 
l = 0 0 1 0 0 
r = 0 0 0 1 1 

After P8, Key-2: 0 1 0 0 0 0 1 1 
_____________________________________________________________________________

Enter e for Encryption | Enter d for Decryption | Enter b for Both
b
Enter 8-bit Plain Text (using space)
1 0 0 1 0 1 1 1

ENCRYPTING..

After IP: 0 1 0 1 1 1 0 1 

After split, 
l = 0 1 0 1 
r = 1 1 0 1 

Round Function(fk)-1
After EP: 1 1 1 0 1 0 1 1 

XOR with key
0 1 0 0 1 1 1 1 

After Split
l = 0 1 0 0 
r = 1 1 1 1 

After S-Box: 1 1 1 1 

After P4
1 1 1 1 

XOR with leftarray
1 0 1 0 

After combine
1 0 1 0 1 1 0 1 

After Swap
l = 1 1 0 1 
r = 1 0 1 0 

Round Function(fk)-2
After EP: 0 1 0 1 0 1 0 1 

XOR with key
0 0 0 1 0 1 1 0 

After Split
l = 0 0 0 1 
r = 0 1 1 0 

After S-Box: 1 1 1 1 

After P4
1 1 1 1 

XOR with leftarray
0 0 1 0 

After combine
0 0 1 0 1 0 1 0 

After IP-Inverse, 8-bit Cipher Text is: 
0 0 1 1 1 0 0 0 
_____________________________________________________________________________
IP
0 0 1 0 1 0 1 0 
Split
0 0 1 0 
1 0 1 0 
Round Function(fk)-1
After EP: 0 1 0 1 0 1 0 1 

XOR with key
0 0 0 1 0 1 1 0 

After Split
l = 0 0 0 1 
r = 0 1 1 0 

After S-Box: 1 1 1 1 

After P4
1 1 1 1 

XOR with leftarray
1 1 0 1 

After combine
1 1 0 1 1 0 1 0 

swap
1 0 1 0 
1 1 0 1 
Round Function(fk)-2
After EP: 1 1 1 0 1 0 1 1 

XOR with key
0 1 0 0 1 1 1 1 

After Split
l = 0 1 0 0 
r = 1 1 1 1 

After S-Box: 1 1 1 1 

After P4
1 1 1 1 

XOR with leftarray
0 1 0 1 

After combine
0 1 0 1 1 1 0 1 

After IP-Inverse, 8-bit Plain Text is: 
1 0 0 1 0 1 1 1 
```
