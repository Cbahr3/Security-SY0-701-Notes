**Key Exchange** - *Out-of-Band Key Exchange* - uses a different trusted communications channel, options include face-to-face meeting, physical mail, telephone call, out-of-band key exchange is difficult and time consuming, *In-Band Key Exchange* - securely exchange keys digitally

**Diffie-Hellman Algorithm** - provides symmetric key exchange capabilities, *p* and *g* must be large values to achieve strong security, ECDH (Elliptic-Curve Diffie-Hellman) utilizes the complexity of the EC formula combined with Diffie Hellman algorithm

**Key Escrow** - allows government access to keys, the Clipper chip included technology that would allow government access to encrypted communications - privacy advocates and industry firms fought strongly against the Clipper chip, *Recovery Agents* - allow internal access to lost keys

**Key Stretching** - takes a relatively insecure value, such as a password, and uses mathematical techniques to strengthen it, making it harder to crack, uses two techniques:
- *Salting* - adds a value to the encryption key to make it more complex
- *Hashing* - adds time to the verification process by requiring more math
Verifying one key is fast, but guessing millions of keys is slow, two common methods of key stretching: 
- *PBKDF2 (Password-Based Key Derivation Function v2)* - uses salting and hashing to stretch a key, should be used at least 4000 times
- *bcrypt* - key stretching with Blowfish

**HSMs (Hardware Security Modules)** - manage encryption keys and perform cryptographic operations, cloud services commonly offer this service, FIPS 140-2 has certain security levels as follows:
- *Security Level 1* - Standard operating systems, no physical security
- *Security Level 2* - EAL2 software and firmware, tamper-evident seals
- *Security Level 3* - EAL3 software and firmware, tamper-resistant controls
- *Security Level 4* - EAL4 software and firmware, strict physical security