**Understanding Wireless Networking** - wireless networking is a constant practice in our lives, the Wi-Fi standard governs communications on many wireless networks, Wi-Fi devices replace network cables with radio transmitters and receivers
- *Wireless Access Points (WAPs)* - connect wireless networks to wired networks and the internet
- Wi-Fi Standards:
	- 802.11n (2009) Wi-Fi 4 allows 600 Mbps communication
	- 802.11ac (2014) Wi-Fi 5 allows 6.9 Gbps communication
	- 802.11ax (2019) Wi-Fi 6 allows 9.6 Gbps communication
Wi-Fi signals travel over open airwaves and are subject to undetectable interception

**Wireless Encryption** - wireless encryption technology prevents eavesdropping attacks
- *Wireless Equivalent Privacy (WEP)* - original wireless encryption standard, contains serious security vulnerabilities, no longer considered secure
- *Wi-Fi Protected Access (WPA)* - replaced WEP in 2003, uses the Temporal Key Integrity Protocol (TKIP) to rapidly rotate encryption keys, contains vulnerabilities, no longer considered secure
- *Wi-Fi Protected Access v2 (WPA2)* - released in 2004 as upgrade to WPA, encrypts packets using AES encryption, uses the CCM protocol, contains some potential security issues, widely used and considered secure
- *Wi-Fi Protected Access v3 (WPA3)* - required on new Wi-Fi devices from 2020 onward, supports CCMP, uses Simultaneous Authentication of Equals (SAE) for key exchange

**Wireless Authentication** - most wireless networks limit access to authorized users
- *Pre-shared Keys* - are the simplest form of wireless authentication
	- *Hexadecimal String* - 64-hexadecimal characters that encode a 256-bit encryption key
	- *Password* - 8-13 ASCII characters that are converted to a 256-bit encryption key using PBKDF2
	- Limitations of Pre-Shared Keys:
		- Changing the network encryption key is a tremendous burden
		- Identifying users and revoking individual user access is impossible
- *Enterprise Authentication* - individual credentials
	- *Lightweight EAP (LEAP)* - insecure protocol that relies upon MS-CHAP
	- *EAP* - broad framework with many variants, some secure, some not
	- *Protected EAP (PEAP)* - tunnels EAP inside an encrypted TLS session
	- EAP Variants:
		- EAP-TLS is secure
		- EAP-TTLS is also secure
		- EAP-FAST is secure
		- EAP-MD5 is insecure
		Make sure you understand the security status of the specific EAP variants in use on your network
- *Captive Portals* - redirect users to an authorization page

**RADIUS**
- *Remote Authentication Dial-In User Service (RADIUS)* - provides a centralized approach for authentication, authorization, and accounting (AAA), remember that a RADIUS client is usually an application server
	- RADIUS Disadvantages:
		- Uses unreliable User Datagram Protocol (UDP)
		- Does not encrypt the entire authentication sequence

**Wireless Signal Propagation** - many factors affect the ability of radio waves to reach users
- *Omnidirectional Antennas* - send a signal in all directions
- *Directional Antennas* - direct all of the power from an access point in a single direction
- *Beamforming* - an 802.11ac feature that steers a network signal in the direction of client devices
Optional access point placement depends on building characteristics
- *Site Survey* - determines optimal AP placement
	- *Heat Maps* - show areas of strong and weak coverage
Avoiding channel overlap reduces interference from other nearby networks, manipulating power levels modifies wireless signal range

**Wireless Networking Equipment** - wireless networks depend on a significant amount of equipment
- *Fat Access Points* - contain all of the hardware and software needed to operate a wireless network
- *Thin Access Points* - rely on wireless controllers for configuration and to serve as the "brains" of the wireless network
	- *Wireless Controllers* - manage configurations, optimize performance, and reduce interference among APs
- *Wi-Fi Analyzers* - search for rogue networks and test wireless security, Aircrack-ng is a popular wireless security testing tool