**Encryption** - protects information from unauthorized disclosure, Cryptography - use of mathematical algorithms to transform information into an encrypted form that is not readable by unauthorized individuals, Encryption - converts info from plaintext to ciphertext vs. Decryption - ciphertext back to plaintext

**Symmetric Encryption** - also known as shared key encryption, encryption and decryption uses the same secret key, best for when there is only two parties, larger groups require more keys, n(n-1) / 2

**Asymmetric Encryption** - Different keys are used for encryption + decryption, keypairs - public and private, if Bob encrypts a message for Alice he uses Alice's public key, Alice would then decrypt using her private key, slower than symmetric encryption

**Goals of Cryptography** - *1. Confidentiality* - data at rest (stored), data in transit (transmitted over network), data in use (processed in memory), *2. Integrity*, *3. Authentication*, *4. Obfuscation* - hiding sensitive data, *5. Nonrepudiation* - verification of origin, only possible with asymmetric cryptography

**Choosing Encryption Algorithms** - do not build your own algorithm unless you know what you are doing, be skeptical of proprietary software encryption algorithms, use encryption algorithms that are proven to be secure, the longer the key length the more secure and hardware demanding it is

**Cryptographic Lifecycles** - algorithms often become insecure as they age, NIST lifecycle - 1. Initiation, 2. Development and Acquisition, 3. Implementation and Assessment, 4. Operations and Maintenance, 5. Sunset

**Data De-identification & Obfuscation** - removing or anonymizing identifying information on datasets, *Hashing* - replaces sensitive fields with hash values - prone to *rainbow table attack* - compares hash values with precomputed hashes, *salting* - uses random values to defeat rainbow tables, *tokenization* - replaces sensitive fields with a random identifier, *masking* - redacts sensitive information from a file