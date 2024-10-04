**RSA (Rivest, Shamir, Adleman)** - early asymmetric encryption, named after three creators, users create RSA key pairs using two large prime numbers, able to distribute public key freely but keep your private key secure, RSA is slow, RSA is more commonly used to exchange symmetric keys, RSA is expired, variable-length key between 1024 and 4096 bits, US authorities recommend a minimum key length of 2048 bits

**PGP (Pretty Good Privacy)** - Phil Zimmerman's asymmetric algorithm, OpenPGP - open-source implementation of PGP, uses both public and private keys, combines both symmetric and asymmetric cryptography, PGP relies upon other encryption algorithms

**Elliptic Curve & Quantum Cryptography** - asymmetric cryptography is based upon the difficulty of solving complex math problems, finding a way to solve the prime factorization problem would break modern cryptography,
- *ECC (Elliptic Curve Cryptography)* - uses the EC discrete log problem (doesn't use prime factorization)
- *Quantum Computing* - uses quantum mechanics principles, Elliptic curve cryptography can't protect against quantum attacks, quantum cryptography may be stronger than any modern approach

**Tor & Perfect Forward Secrecy - the Tor protocol facilitates an anonymous internet
- *Tor* - the Onion Router (Tor) is a software package that uses encryption and relay nodes to facilitate anonymous internet access
- *Perfect Forward Secrecy* - hides nodes' identity from each other