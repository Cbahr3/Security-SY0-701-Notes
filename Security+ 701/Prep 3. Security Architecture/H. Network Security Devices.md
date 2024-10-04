**Routers, Switches, and Bridges** - routers, switches, and bridges are the building blocks of computer networks
- *Switches* - connect devices to the network, switches reside in wiring closets and connect the computers in a building together, switches typically work at Layer 2 - Data Link Layer, switches may function at Layer 3 - Network Layer
- *Ethernet Jacks* - are at the other end of network cables connected to switches
- *Wireless Access Points (WAPs)* - connect to switches and create Wi-Fi networks
- *Routers* - connect networks to each other, making intelligent packet routing decisions
- *Bridges* - connect networks using simple forwarding

**Firewalls**
- *Firewalls* - serve as the security guards at the perimeter of a network
- *Screened Subnet* - contains systems that must accept direct external connections, isolates those systems due to risk of compromise, protects internal network from compromised screened subnet systems
- *Stateless Firewall* - evaluates each connection independently
- *Stateful Inspection* - tracks open connections
- Firewall Rule Contents:
	- Source system address
	- Destination system address
	- Destination port and protocol
	- Action (allow or deny)
- *Implicit Deny* - if the firewall receives traffic not explicitly allowed by a firewall rule, then that traffic must be blocked
- *Next-generation Firewalls (NGFWs)* - incorporate contextual information into their decision-making, they are also known as layer 7 firewalls
- Other Firewall Roles:
	- NAT gateway
	- Content/URL filtering
	- Web application firewall
- Firewall Deployment Options:
	- Network hardware vs. host-based software
	- Open source vs. proprietary
	- Hardware appliance vs. virtual appliance

**Web Application Firewalls**
- *Web Application Firewall* - screens web connections
	- WAFs Protect Against:
		- SQL injection
		- Cross-site scripting
		- Directory traversal
		- Buffer overflows
		- Privilege escalation
		- Cookie-based attacks
	- *Hardware WAF* - physical device positioned between the network firewall and web server
	- *Software WAF* - software running on the web server that screens requests
	- *Cloud-Based WAF* - third-party service that remotely filters malicious traffic, cloud-based WAFs are particularly effective against denial-of-service attacks
	- *XML Firewall* - filters access to REST APIs
Web application firewalls are an important component of a defense-in-depth cybersecurity strategy

**Proxy Servers**
- *Proxy Servers* - connect to websites on a user's behalf
	- Proxy Server Benefits:
		- Anonymization
		- Performance boosting
		- Content filtering
	- *Forward Proxies* - work on behalf of clients
	- *Reverse Proxies* - work on behalf of servers
	- *Transparent Proxies* - work without the client's or server's knowledge
Proxies can handle many applications, not just web traffic

**Load Balancers**
- *Load Balancers* - distribute work among servers
	- *Autoscaling* - automatically adds and removes servers, as needed
	- Load Balancer Security Functions:
		- SSL certificate management
		- URL filtering
		- Other web application security tasks
	- *Round-Robin Scheduling* - each server gets an equal number of requests
	Advanced scheduling algorithms choose servers based upon performance and available capacity
	- *Session Persistence* - routes an individual user's requests to the same server
	- *Active-Active* - two or more load balancers actively handle network traffic and continue to function with diminished capacity if one device fails
	- *Active-Passive* - one load balancer handles all traffic while a second monitors activity and assumes responsibility if the primary load balancer fails

**VPNs and VPN Concentrators**
- *Site-to-Site VPNs* - connect remote offices to each other and headquarters
- *Remote Access VPNs* - provide remote access to corporate networks for mobile users
- VPN Endpoints:
	- Firewalls
	- Routers
	- Servers
	- VPN concentrators
- *IPsec* - works at the network layer (Layer 3), supports the Layer 2 Tunneling Protocol (L2TP), provides secure transport, difficult to configure
SSL/TLS VPNs work at the application layer over TCP port 443, HTML5 VPNs work entirely within the web browser
- *Full-Tunnel VPN* - all network traffic leaving the connected device is routed through the VPN tunnel, regardless of its final destination
- *Split-Tunnel VPN* - only traffic destined for the corporate network is sent through the VPN tunnel, other traffic is routed directly over the internet, split-tunnel VPNs provide users with a false sense of security
- *Always On VPN* - connects automatically

**Network Intrusion Detection and Prevention**
- *Intrusion Detection Systems (IDS)* - monitor network traffic for signs of malicious activity
	- Intrusion Detection Systems:
		- Alert administrators to suspicious activity
		- Require someone to monitor and take appropriate action
- *Intrusion Prevention System (IPS)* - block malicious activity automatically
- IDS and IPS systems are prone to two types of errors:
	- *False Positive Error* - IDS/IPS triggers an alert when an attack did not actually take place
	- *False Negative Error* - IDS/IPS fails to trigger an alert when an actual attack occurs
- *Signature Detection Systems*:
	- Contain databases with rules describing malicious activity
	- Alert administrators to traffic matching signatures
	- Fail to detect brand new attacks
- *Anomaly Detection Systems*:
	- Build models of "normal" activity trends
	- Alert administrators to activity not matching the trend
	- Detect previously unknown attacks
	- Increased false positive rates
	Anomaly detection, behavior-based detection, and heuristic detection are all the same thing
	- IPS Deployment Modes:
		- *Inline (active) Deployments* - device sits in the path of network communications, device can block suspicious traffic from entering the network
		- *Out-of-Band (passive) Deployments* - device connects to a SPAN or TAP port on a switch, device can react after suspicious traffic enters the network

**Protocol Analyzers**
- *Protocol Analyzers* - allow deep inspection of traffic
	- Protocol Analyzer Uses:
		- Troubleshoot network issues
		- Investigate security incidents
		- Eavesdrop on confidential communications
	- *tcpdump* - open-source command-line protocol analyzer
Wireshark and tcpdump are both built on the libpcap library
- *tcpreplay* - allows editing and replaying traffic

**Unified Threat Management**
- *Unified Threat Management (UTM) Solutions* - combine multiple security functions in a single appliance
	- Basic UTM Functions:
		- Protecting network against attacks
		- Blocking unsolicited traffic
		- Routing traffic to and from the internet
	- Additional Security Features:
		- VPN connectivity
		- Intrusion detection
		- Intrusion prevention
	- Small Business Features:
		- URL filtering
		- Content inspection
		- Malware inspection
		- Email and spam filtering
UTM devices still require regular monitoring

**Failure Modes** - security engineering ensures that systems meet both business and security requirements
- *Security Is a Design Element* - "Bolt-on" security rarely works
- Failure Modes:
	1. *Fail open* - failed security controls are bypassed
	2. *Fail closed* - failed security controls block access