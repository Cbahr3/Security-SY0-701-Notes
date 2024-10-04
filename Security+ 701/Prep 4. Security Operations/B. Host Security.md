**Operating System Security** - administrators should configure endpoint operating systems to meet organizational security requirements, limit administrative access to systems
- *Patch Management* - corrects security issues
Use configuration management tools to patch operating systems and applications
- *System Hardening* - locks down configurations, remove unnecessary software and system components, lock down the host firewall configuration, disable default accounts and passwords, confirm Windows registry and Linux configuration settings match best practices

**Malware Prevention**
- *Viruses*- spread by human action
- *Worms* - spread by themselves
- *Trojan Horses* - disguise themselves
- *Spyware* - gathers information
Antimalware software protects against many different threats
- *Signature Detection* - watches for known patterns of malware activity
- *Behavior Detection* - watches for deviations from normal patterns of activity
- *Endpoint Detection and Response (EDR)* - offers real-time, advanced protection
	- *Sandboxing* - isolates malicious content
- *Spam Filtering* - blocks unwanted email
Malware logs should be sent to a centralized system for storage and analysis

**Application Management**
- *Application Control* - restricts what software may run
	- *Allow Lists* - administrators create a list of all the applications that may run on a system
	- *Deny Lists* - administrators create a list of the applications that are prohibited on a system
Send application control logs to your SIEM or log repository for analysis
- *Host Software Baselining* - identifies expected system software

**Host-based Network Security Controls**
- *Default Deny Rule* - firewalls, by default, block any network connection attempts that are not explicitly allowed by a firewall rule
- *Network Firewalls* - hardware devices that regulate connections between two networks
- *Host Firewalls* - software components of an operating system that limit connections to a server
Granting network access requires configuring both network and host firewalls
- *Next-Generation Firewall (NGFW)* - incorporates advanced security features, such as contextual information about the user and application
- *Intrusion Detection System (IDS)* - alerts administrators to suspicious network activity
- *Intrusion Prevention System (IPS)* - takes proactive measures to block suspicious network activity
Intrusion detection and prevention capabilities are found in third-party security solutions, send host firewall and host IDS and IPS logs to your SIEM or log repository for analysis

**File Integrity Monitoring** - defense-in-depth strategies require the use of diverse, overlapping security controls
- *File Integrity Monitoring (FIM)* - watches for unexpected file modifications
	- *Hash Function* - hash functions are one-way functions that transform a variable-length input into a unique, fixed-length output
	File integrity monitoring systems periodically verify that the hash values of critical files have not changed, tuning is critical, adjust the FIM system for your organization's needs

**Data Loss Prevention** - organizations routinely handle sensitive information
- *Data Loss Prevention (DLP)* - technology solutions that search systems and monitor networks for unsecured sensitive information and provide the ability to remove the information, block the transmission, or encrypt the stored data
	- Placements of DLP:
		- *Host-Based DLP* - uses software agents installed on a single system
		- *Network-Based DLP* - scans network transmissions for sensitive information
	- Techniques of DLP:
		- *Pattern Matching* - recognizes known patterns of sensitive information, such as Social Security numbers
		- *Watermarking* - identifies sensitive information using electronic tags
	Cloud-based DLP systems operate as managed security services

**Data Encryption** - encryption protects sensitive data by transforming it so that it may not be read by anyone without the appropriate decryption key
- *Key Management System (KMS)* - manages the creation, distribution, management, and disposal of encryption keys in a secure manner
- *AES Crypt* - open-source file encryption
- *Full-Disk Encryption* - protects an entire drive
- *Hardware Security Module (HSM)* - manages encryption keys
- *Trusted Platform Modules (TPMs)* - bring hardware encryption to typical computers
- *Self-Encrypting Drives (SED)* - perform encryption automatically

**Hardware and Firmware Security** - operating systems must be loaded from disk during the boot process
- *Basic Input/Output System (BIOS)* - lightweight operating system stored in firmware that provides the basic functionality necessary to load the full operating system from disk
BIOS attacks may give a malicious individual full control of a device
- *Unified Extensible Firmware Interface (UEFI)* - replaces BIOS with a flexible alternative
	- *Secure Boot*
		1. Read the boot loader from disk
		2. Compute the hash of the boot loader
		3. Decrypt the boot loader's digital signature
		4. Verify that the signature is accurate
	Booting stops abruptly if the boot loader's digital signature fails verification, remote attestation sends a compliance report to an external server
- *Measured Boot* - each device verifies the hash of the next device in the boot chain
	- *Attestation* - confirmed hashes are stored in the TPM
- *Hardware Root of Trust* - verifies firmware integrity
Together, the hardware root of trust, UEFI, TPM, and Secure Boot provide trusted execution
- *Bus Encryption* - protects inter-component communication
- *Secure Enclaves* - provide hardware-based encryption key management
- *Processor Security Extensions* - allow applications to request their own protected areas of memory
- *Atomic Execution* - guarantees "all-or-nothing" transaction execution
- *Electromagnetic Interference (EMI)* - electromagnetic waves, normally generated unintentionally, that cause disruption to nearby electronic equipment
	- *Electromagnetic Pulses (EMPS)* - are extreme bursts of EMI, they may be generated by a nuclear explosion

**Linux File Permissions**
- Linux File System Access Commands:
	- *chown* - changes a file or directory user owner
	- *chgrp* - changes a file or directory group owner
	- *chmod* - changes the permissions on a file or directory
- Linux Permissions
	- File Permissions:
		- Read (r)
		- Write (w)
		- Execute (x)
	- File Ownerships:
		- User owner (u)
		- Group owner (g)
		- Others (o)

**Web Content Filtering**
- *Web Content Filtering* - controls access to websites
	- *Agent-Based* - installs a filtering agent directly on end-user devices
	- *Centralized Proxy* - routes all website requests through a centralized proxy server that performs filtering
	- *URL Scanning* - analyzes URLs to identify those that are harmful or unwanted
	- *Filters* - use site categorization to determine the topic(s) of a website
	- *Block Rules* - restrict access to a specific site or page
	- *Site Reputation Data* - informs content filtering decisions