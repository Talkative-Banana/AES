# AES
Advanced Encryption Algorithm

# Project Overview
This project implements the Advanced Encryption Standard (AES) algorithm to perform encryption and decryption on 128-bit plaintext. We developed two main programs for this task: one for encryption and one for decryption. This AES implementation uses 10 rounds of encryption and decryption, applying key expansion and various transformations according to the AES specification.

# Table of Contents
- Introduction
- Project Structure
- AES Algorithm Overview
- Encryption Steps
- Decryption Steps
- How to Run
- Examples
- Authors

# Introduction
The AES encryption standard is widely used in securing digital data. It involves multiple rounds of transformations to produce ciphertext from plaintext and vice versa. Our project focuses on implementing AES encryption and decryption with a 128-bit block size and a 128-bit key, involving specific transformations for each round.

## Project Structure
    ├── main.py                   # Encryption and Decryption
    └── README.md                 # Project README file
## AES Algorithm Overview
AES encryption and decryption include the following key transformations applied over 10 rounds:

## Encryption Steps
- Substitution Bytes - Substitute bytes using an S-box.
- Shift Rows - Shift rows of the state array.
- Mix Columns - Mix columns through matrix multiplication in GF(2^8).
- Add Round Key - XOR with the round key.

## Decryption Steps
- Inverse Shift Rows - Reverse row shifts.
- Inverse Substitution Bytes - Substitute bytes using the inverse S-box.
- Add Round Key - XOR with the round key.
- Inverse Mix Columns - Perform inverse column mixing.

## How to Run
Clone the repository:

```
git clone https://github.com/Talkative-Banana/AES.git
cd AES
run .pynb file
```
## Examples
### Encryption
```
Input Plaintext: 00112233445566778899aabbccddeeff
Key: 000102030405060708090a0b0c0d0e0f
Encrypted Ciphertext: 69c4e0d86a7b0430d8cdb78070b4c55a
```
### Decryption
```
Input Ciphertext: 69c4e0d86a7b0430d8cdb78070b4c55a
Key: 000102030405060708090a0b0c0d0e0f
Decrypted Plaintext: 00112233445566778899aabbccddeeff
```
## Authors
Ekansh - IIIT Delhi

Lakshay Bansal - IIIT Delhi
