**Denial-Of-Service Attacks**
- *DoS (Denial-of-Service Attack)* - makes a resource unavailable for legitimate use, sends a huge number of requests to a server, is difficult to distinguish from legitimate requests, limitations include:
	- Requires a massive amount of bandwidth
	- Is easy to block based on IP address
- *DDoS (Distributed Denial of Service)* - a denial-of-service attack that leverages a botnet to overwhelm a target
	- *The Amplification Factor* - the degree to which the attack increases in size, reply / request = amplification
- DoS Variants:
	- Network attacks
	- Application attacks
	- OT (Operational Technology) attacks
Defending against DDoS attacks is often done by service providers

**Eavesdropping Attacks**
- *Eavesdropping Attacks* - rely on a compromised communications path
	- Network device tapping
	- DNS poisoning
	- ARP poisoning
- Types of eavesdropping attacks:
	- *Man-in-the-Middle Attack* - user connects directly to the attacker, attacker in turn connects with the target server, can view all the communications that take place between the client and the server
	- *Man-in-the-Browser Attack* - exploits flaws in browsers and browser plugins, man-in-the-middle attacks and man-in-the-browser attacks are on-path attacks
	- *Replay Attack* - uses previously captured data to create a separate connection to the server, the attacker can't see the encoded credentials, preventing replay attacks involves:
		- Include a unique characteristic
			- Token
			- Timestamp
		- Prevent reuse of captured credentials
	- *SSL Stripping* - tricks browsers into using unencrypted communications

**DNS Attacks**
- *DNS (Domain Name System)* - a service that translates common domain names into IP addresses for the purpose of network routing
- *Typosquatting* - an attack that consists of registering domain names similar to official sites, hoping that users will make a typo and visit their site
- *Domain Hijacking* - an attack where the attacker gains control of an organization's domain registration
- *URL Redirection* - attacker places redirects on trusted site to content hosted on a malicious site
- *Domain Reputation* - threat intelligence capability that scores domains as either benign or malicious

**Wireless Attacks**
- *WEP (Wired Equivalent Privacy)* - is inherently insecure, WEP attacks depend on capturing (IVs) initialization vectors
- *WPA (Wi-Fi Protected Access) Security* - WPA, like WEP, depends on RC4, WPA adds the TKIP (Temporal Key Integrity Protocol), WPA is no longer considered secure, WPA2 and WPA3 are secure alternatives
- *WPS (Wi-Fi Protected Setup)* - WPS allows quick setup of devices
	- There are two methods for establishing connection:
		- Pressing buttons on devices
		- Using the eight-digit WPS PIN
	- WPS Attacks:
		- Flaws in WPS make it trivial to guess the WPS PIN
		- Though there are 10,000,000 possibilities, a flaw requires only 11,000 guesses
		- If you guess the PIN, you get the encryption key
		- PIN can't be changed
		- Disable WPS!

**Propagation Attacks** - wireless networks are vulnerable to eavesdropping attacks
- *Jamming and Interference* - denial-of-service attacks are easy on wireless, the radio spectrum is open, the loudest signal always wins, so it doesn't take much to interfere with another signal
- *Wardriving Attacks* - attackers will cruise neighborhoods and commercial areas, using tools that capture information about Wi-Fi networks
	- *Warflying Attacks* - take wardriving airborne

**Preventing Rogues and Evil Twins**
- *Rogue Access Points* - occur when someone connects an unauthorized wireless access point to an enterprise network
	- Rogue Access Point Risks:
		- Bypassing authentication
		- Interference
	- Rogue Access Point Detection:
		- Enterprise-grade wireless has built-in intrusion detection capabilities
		- Unknown radios on the network can be identified
		- Handheld tools can also help pinpoint them
- *Evil Twin Attacks* - hacker sets up a fake access point with the SSID of a legitimate network, they then lure unsuspecting visitors when they're in the vicinity, since the hacker controls the network they can use DNS poisoning and similar tactics to redirect users to phishing websites

**Disassociation Attacks** - disassociation attacks speed up other wireless attacks
- *Disassociation* - wireless access points may force a wireless device to immediately disconnect from the network, normally clients stay connected to wireless networks for extended periods of time
	- Goals:
		- Gather authentication information for cryptographic attacks
		- Conduct denial-of-service attacks on wireless networks

**Understanding Bluetooth Attacks** - Bluetooth is commonly used to connect devices and peripherals over short distance
- *Bluejacking* - an attacker sends Bluetooth spam to a user's device, the attacker tries to entice the user to take some action, this is essentially Bluetooth spam/phishing
- *Bluesnarfing* - an attacker exploits a firmware flaw in older Bluetooth devices. the attacker forces pairing between devices, the connection grants access to the device
- Bluetooth Security:
	- Turn off discoverable mode when not in use
	- Apply firmware updates
	- Watch for suspicious activity

**RFID Security** - RFID chips are embedded in many items and may be read by RFID scanners
- Common uses of RFID technology include:
	- Passports bearing the international standard electronic passport symbol contain RFID chips
	- Transit cards and credit cards often contain RFID chips to allow contactless reading
	- Electronic toll systems use RFID
	- Warehouses track inventory with RFID
- RFID Security Concerns:
	- Businesses want strong authentication and encryption to protect the integrity of RFID systems and prevent RFID cloning
	- Consumers want privacy safeguards to protect their personal information