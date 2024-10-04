**Trust Models** - strong cryptography always depends upon some degree of trust, the two parties must be confident that they are really communicating with each other and that neither one is an imposter, the two parties must be confident that nobody is eavesdropping on the key exchange, in asymmetric cryptography users don't need to share their private keys and they can (and should) share their public keys freely, in asymmetric encryption eavesdropping protection isn't needed during key exchange but we still need to prevent imposters, three ways to increase trust: 
- *Personal knowledge*
- *Web of trust (WOT)* - relies on indirect relationships, participants digitally sign the public keys of people they know personally, issues include decentralized approach, high barrier to entry, requires technical knowledge
- *Public key infrastructure (PKI)* - builds upon the web of trust

**PKI and digital certificates** - the PKI depends upon highly trusted certificate authorities (CAs)
- *CA (Certificate Authority)* - trusted third-party organizations that verify the identity of individuals or organizations and then issue digital certificates containing both identity information and a copy of the subject's public key
Digital certificates are the identity cards of the digital world, anyone receiving your digital certificate can verify its authenticity by checking the digital signature of the issuing CA

**Hash Functions** - one-way function that transform a variable length input into a unique, fixed-length output, characteristics include:
- One-way functions can't be reversed
- The output of a hash function will always be the same length, regardless of the input size
- No two inputs to a hash function should produce the same output
Hash functions can fail if:
- If they are reversible
- If they are not collision resistant
Types of hash functions include:
- *MD5 (Message Digest 5)* - created in 1991, the fifth in a series of hash functions, message digest is another term for hash, MD5 produces 128-bit hashes. MD5 is no longer secure
- *SHA (Secure Hash Algorithm)* - created by NIST as a government standard
	- *SHA-1* - produces a 160-bit hash value, contains security flaws that render it insecure
	- *SHA-2* - consists of a family of six hash functions, produces output of 224, 256, 384, and 512 bits, uses a mathematically similar approach to SHA-1 and MD5
	- *SHA-3* - designed to replace SHA-2, uses a completely different hash generation approach than SHA-2, produces hashes of user-selected fixed length
- *RIPEMD (Race Integrity Primitives Evaluation Message Digest)* - created as an alternative to government-sponsored hash functions, produces 128, 160, 256, and 320-bit hashes, contains flaws in the 128-bit version
*HMAC (Hash-based Message Authentication Code)* - combines symmetric cryptography and hashing, provides authentication and integrity, create and verify message authentication code by using a secret key in conjunction with a hash function, hash functions are used with asymmetric cryptography for digital signatures and digital certificates

**Digital Signatures** - use asymmetric cryptography to achieve integrity, authentication, and nonrepudiation, signed message recipients know:
1. The owner of the public key is the person who signed the message.
2. The message was not altered after being signed.
3. The recipient can prove these facts to a third party.
Digital signatures depend upon:
- Collision-resistant hash functions
- Asymmetric cryptography
Digital signatures are created using your private key, digitally signing messages does not provide confidentiality

**Digital Signature Standard** - Approved DSS Algorithms:
- RSA (Rivest-Shamir-Adleman)
- ECDSA (Elliptic Curve Digital Signature Algorithm)
- EdDSA (Edwards Curve Digital Signature Algorithm)

**Create a Digital Certificate** - digital certificates follow the X.509 standard, digital certificates include common certificate attributes - certificate subject's public key, expiration date, and Common Name attribute, certificates allow the inclusion of SANs (Subject Alternative Names)

**Revoke a Digital Certificate** - *Certificate Revocation* - invalidates compromised certificates, two methods for revoking a certificate:
- *CRL (Certificate Revocation List)* - includes serial numbers of revoked certificates
- *OCSP (Online Certificate Status Protocol)* - provides real-time certificate status verification

**Certificate Stapling** - OCSP places a significant burden on the OCSP servers operated by certificate authorities (CAs), *Certificate Stapling* - reduces the CA's burden, stapled certificates are often valid for 24 hours

**Certificate Authorities** - users verify the digital certificate's authenticity using the CA's public key, CAs charge fees for their services when creating a new certificate
- *Self-Signed Certificates* - issued by an internal CA
- *Certificate chaining* - allows the use of intermediate CAs
- *Offline CAs* - protect sensitive root keys

**Certificate Subject** - owner of the public key, could be any of the following:
- Servers - web, SSH, file, email, etc.
- Devices - SANs, routers, switches, VPNs, access points, etc.
- Individuals - names, email addresses
- Developers - for code signing
*Certificate Pinning* - ties a certificate to a subject for a period of time

**Certificate Types**
- *Root Certificates* - protect CA private keys
- *Wildcard Certificates* - cover an entire domain
	- x.linkedin.com
		- www.linkedin.com
		- mail.linkedin.com
		- secure.linkedin.com
	- Wildcard certificates only match one level deep, wildcard certificates are commonly used for load balancers
CAs issuing certificates are vouching for the certificate subject's identity, there are three types of verification that may be used:
- *Domain Validation* - verifies domain ownership
- *Organizational Validation* - verifies business name
- *Extended Validation* - requires extensive investigation

**Certificate Formats** - certificates come in different formats:
- *DER (Distinguished Encoding Rules)* - binary format, use DER, CRT, and CER file extensions
- *PEM (Privacy Enhanced Mail)* - ASCII text equivalents of DER certificates, convert with OpenSSL, use PEM and CRT extensions. CRT files may be either DER binary certificates or PEM text certificates
- *PFX (Personal Information Exchange)* - binary format, commonly used by Windows systems, use PFX and P12 file extensions
- *P7B Format* - ASCII text equivalent of PFX certificates, commonly used by Windows systems, uses P7B file extension