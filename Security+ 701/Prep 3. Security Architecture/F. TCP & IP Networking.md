**Introducing TCP/IP** - networks carry many types of sensitive information
- *IP (Internet Protocol)* - routes information across networks, providing an addressing scheme, deliver packets from source to destination, serves as a network layer protocol
- *TCP (Transmission Control Protocol* - is a connection-oriented protocol, guarantees delivery through acknowledgment, is widely used for critical applications
	- TCP Flags:
		- *SYN* - opens a connection
		- *FIN* - closes a connection
		- *ACK* - acknowledges a SYN or FIN
- *UDP (User Data Protocol)* - is a lightweight, connectionless protocol, doesn't send acknowledgments or guarantee delivery, is used for voice and video applications
- *OSI Model*:
	1. *Physical Layer* - wires, radios and optics
	2. *Data Link Layer* - data transfers between two nodes
	3. *Network Layer* - IP (Internet Protocol)
	4. *Transport Layer* - TCP and UDP
	5. *Session Layer* - exchanges between systems
	6. *Presentation Layer* - data translation and encryption
	7. *Application Layer* - user programs

**IP Addresses and DHCP** - IP addresses facilitate the delivery of network traffic
- *IP Addresses* - uniquely identify systems
	- Why the Range 0-255?:
		- 8-bit binary numbers
		- 2^8 = 256 possible values
		- Start counting at 0
		- Range: 0-255 (256 values)
	- IP Addresses:
		- Uniquely identify systems on a network
		- Must not be reused on internet-connected systems
		- May be reused if on private networks
	- IPv6:
		- Replaces IPv4 due to address exhaustion
		- Uses 128 bits (compared to 32 for IPv4)
		- Consists of eight groups of four hexadecimal numbers
	- *Static IPs* - static IPs are manually assigned to systems by an administrator, they must be unique and within the appropriate range for the network
	- *DHCP (Dynamic Host Configuration Protocol)* - the DHCP (Dynamic Host Configuration Protocol) allows the automatic assignment of IP addresses from an administrator-configured pool

**DNS (Domain Name Service)**
- *DNS* - provides address resolution on the internet, DNS functions over UDP port 53
- *DNS Servers* - translate between domain names and IP addresses
- DNS Resolution:
	1. User types domain name into browser
	2. Computer sends a DNS query to the local DNS server
	3. DNS server responds with an IP address
	4. Computer contacts the server at that IP address
DNS is a hierarchical system - organizations designate servers that are authoritative for their domains, some content filters alter DNS query results
- *DNSSEC* - adds digital signatures to DNS

**Network Ports** - network ports, like apartment numbers, guide traffic to the correct final destination
- Network Port Numbers:
	- 16-bit binary numbers
	- 2^16 or 65,536 possible values
	- Start counting at 0
	- Allowable range of 0-65,535
- Port Ranges:
	- 0-1,023: well-known ports
	- 1,024-49,151: registered ports
	- 49,152-65,535: dynamic ports
- Administrative Services:
	- Port 21: File Transfer Protocol (FTP)
	- Port 22: Secure Shell (SSH)
	- Port 3389: Remote Desktop Protocol (RDP)
	- Ports 137, 138, and 139: NetBIOS
	- Port 53: Domain Name Service (DNS)
- Mail Services:
	- Port 25: Simple Mail Transfer Protocol (SMTP)
	- Port 110: Post Office Protocol (POP)
	- Port 143: Internet Message Access Protocol (IMAP)
- Web Services:
	- Port 80: Hypertext Transfer Protocol (HTTP)
	- Port 443: Secure HTTP (HTTPS)

**ICMP**
- *ICMP (Internet Control Message Protocol)* - is the housekeeping protocol of the internet
	- *Ping* - identifies live systems
	- *Traceroute* - identifies network paths
	- Other ICMP Functions:
		- Destination unreachable
		- Redirects
		- Time exceeded
		- Address mask requests and replies