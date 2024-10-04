**TLS and SSL** - digital certificates allow the secure exchange of public keys
- *Transport Layer Security (TLS)* - encrypts network communications
- *Secure Sockets Layer (SSL)* - insecure predecessor to TLS
- *OpenSSL* - open-source TLS project
- *SSL Inspection* - performs a "friendly" man-in-the-middle attack to inspect network traffic

**IPSec** - the original implementation of TCP/IP didn't consider security
- *Internet Protocol Security (IPSec)* - IPSec secures the entire packet payload
	- *Encapsulating Security Payload (ESP)* - provides confidentiality and integrity protection for packet payloads
	- *Authentication Header (AH)* - provides integrity protection for packet headers and payloads
	You can combine ESP and AH
	- *Security Association (SA)* - identifies cryptographic algorithms
	- *Site-to-Site VPNs* - encrypted tunnels connecting two networks together in a manner that is transparent to users, this use of IPSec is known as Tunnel mode
	- *End-User VPNs* - provide encrypted remote network access for individual systems, this use of IPSec is known as Transport mode

**Securing Common Protocols** - many common protocols do not include built-in security
- *HTTPS* - adds TLS to web browsing
Telnet uses insecure command-line access, SSH is a secure alternative
- File Transfers:
	- FTP is insecure
	- FTP Secure/FTP over SSL (FTPS) adds TLS to FTP
	- Secure FTP/SSH FTP (SFTP) transfers files over SSH
	- Secure Copy (SCP) provides secure command-line file transfer over SSH
	- The Trivial File Transfer Protocol (TFTP) is rarely used and is not secure
Voice and video communications should leverage TLS encryption whenever possible, RTP-based VoIP services should use the secure SRTP protocol
- *Network Time Protocol* - synchronizes system clocks, secure version is NTPsec
- Email Protocols:

| Protocol | Unencrypted Port | Encrypted Port |
| -------- | ---------------- | -------------- |
| POP      | 110              | 995            |
| IMAP     | 143              | 993            |
| SMTP     | 25               | 587            |
	Encrypt email messages and attachments with S/MIME
- Secure Networking Protocols:
	- USE DNSSEC to add digital signatures to DNS
	- Limit authorized DHCP servers
	- LDAPS offers a secure alternative to LDAP

**DKIM, DMARC, and SPF**
- *Sender Policy Framework (SPF)* - SPF provides domain owners with the ability to list the servers that are authorized to send mail from the domain
- *DomainKeys Identified Mail (DKIM)* - DKIM provides email authentication by allowing mail servers to digitally sign legitimate outbound email messages, DKIM uses public-private key pairs, public keys are published through DNS
- *Domain-based Message Authentication, Reporting, and Conformance (DMARC)* - provides domain owners with the ability to specify SPF and DKIM policies for their domains

**Email Gateways** - email remains a crucial tool for the modern business
- *Email Gateways* - monitor and filter inbound and outbound email, email gateways integrate with other tools and protocols, such as DMARC, DKIM, and SPF, email gateways enforce an organization's data-sharing policies, email gateways incorporate artificial intelligence and other advanced techniques