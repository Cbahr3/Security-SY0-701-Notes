**DES (Data Encryption Standard)** - created by IBM in 1970, intended to serve as federal encryption standard, no longer considered secure, used for symmetric encryption, block cipher operating on 64-bit blocks, key length of 56 bits, 2048 bits or higher is considered secure

**3DES (Triple DES)** - applies DES encryption three times, *Keying Option 1* - K1 ≠ K2 ≠ K3, *Keying Option 2* - K1 = K3, K1 ≠ K2, K2 ≠ K3, *Keying Option 3* - K1 = K2 = K3, Double DES in no more secure than standard DES due to the meet-in-the-middle attack, Triple DES is being phased out, used for symmetric encryption, block cipher operating on 64-bit blocks, effective key length of 112 bits, considered weak now

**Other Encryption Algorithms**
- *AES (Advanced Encryption Standard)* - replaced DES, uses substitution and transposition, symmetric encryption algorithm, block cipher operating on 128-bit blocks, key length of 128, 192, or 256 bits, considered secure
- *Blowfish* - public domain algorithm, designed as a DES replacement, uses a Feistel network, combines substitution and transposition, used for symmetric encryption, block cipher operating on 64-bit blocks, key length anywhere between 32 and 448 bits, not considered secure
- *Twofish* - Designed as a DES replacement, placed into the public domain, uses a Feistel network, combines substitution and transposition, used for symmetric encryption, block cipher operating on 128-bit blocks, key length of 128, 192, or 256 bits, considered secure

**Steganography** - hides data in large files, often uses innocent-looking high-resolution images - slight modifications to image pixels may hide information, may also be used with audio and video files