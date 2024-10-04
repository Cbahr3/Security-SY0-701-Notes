**Preventing SQL Injection** - dynamic web applications depend upon back-end databases, applications request data from databases using SQL (Structured Query Language), prevention techniques for SQL injection include:
- *Input Validation* - protects against unsafe user input by checking it on the server before executing commands
- *Parameterized SQL* - precompiles SQL code on the database server to prevent user input from altering query structure

**Understanding Cross-Site Scripting**
- *XSS (Cross-Site Scripting)* - cross-site scripting attacks occur when an attacker embeds malicious scripts in a third-party website that are later run by innocent visitors to that site, XSS attackers embed scripts in sites without permission
- *HTML* - enhances websites with formatting and images
	- *HTML Tags* - mark up text with formatting instructions, < b >, < i >, < script > for example
- Use input validation to stop XSS - don't allow < script > tags in user-supplied input

**Request Forgery** - cross-site request forgery attacks pose a risk to web applications
- Cross-site request forgery, CSRF, XSRF, and "sea surf" all refer to the same attack
- *Cross-Site Request Forgery* - cross-site request forgery (CSRF or XSRF) attacks leverage the fact that users are often logged into multiple sites at the same time and use one site to trick the browser into sending malicious requests to another site without the user's knowledge, CSRF is a client-side attack
	- XSRF secretly sends requests often using image tags
	- Defending Against CSRF
		- Rearchitect web applications
		- Prevent the use of HTTP GET requests
		- Advise users to log out of sites
		- Automatically log out users after an idle period
- *SSRF (Server-Side Request Forgery (SSRF)* - request forgery attack that targets servers, rather than users, by manipulating servers into retrieving malicious data from what it believes to be a trusted source

**Overflow Attacks** - developers set aside areas of memory called buffers to store user-supplied content
- *Buffer Overflow Attacks* - use input larger than the buffer

**Explaining Cookies and Attachments** - cookies track user activity on the web
- *Cookies* - cookies are data stored by websites in user browsers, they are particularly useful to recognize users, they are used to remember information, privacy risks related to cookies include:
	- Cookies can be used across different websites
	- Cookies can track user activity
	- If you log into one site, everything is de-anonymized

**Session Hijacking** - cookies provide an easy shortcut for web authentication
- *Guessable Cookies* - jeopardize security
- Possible issues with cookies include:
	- *Cookie Guessing* - possible if cookie values are not randomly generated
	- *Session Replay* - possible if cookie values are not encrypted in transit
- *Secure Cookies* - sent using encryption

**Code Execution Attacks**
- *Code Execution Attacks* - occur when an attacker exploits a vulnerability in a system that allows the attacker to run commands on that system
	- *Arbitrary Code Execution* - code execution attacks where the attacker runs commands of his or her choice
	- *Remote Code Execution* - code execution attacks that take place over a network connection
	- Code Execution Objectives:
		- Install malicious code
		- Join a system to a botnet
		- Steal sensitive information
	- Steps to Protect Systems Against Code Execution Attacks:
		1. Limit administrative access
		2. Patch systems and applications

**Privilege Escalation**
- *Privilege Escalation Attack* - gains administrative access, privilege escalation attacks often exploit buffer overflow vulnerabilities, mitigating privilege escalation involves:
	- Perform input validation
	- Patch operating systems, platforms, and applications
	- Enforce the least privilege principle
	- Use DEP (Data Execution Prevention) and ASLR (Address Space Layout Randomization) technologies

**OWASP Top Ten** - the OWASP (Open Worldwide Application Security Project) maintains a list of common web security issues
- *Broken Access Control* - allows unauthorized access
- *Cryptographic Failures* - allow access to sensitive data
- *Injection* - inserts unwanted code
- *Insecure Design* - fails to meet security requirements
- *Security Misconfiguration* - occurs in many possible locations
- *Vulnerable and Outdated Components* - jeopardize application security
- *Identification and Authentication Failures* - allow exploitation of session management
- *Software and Data Integrity Failures* - allow insertion of insecure code
- *Security Logging and Monitoring Failures* - deprive analysts of needed data
- *SSRF (Server-Side Request Forgery)* - tricks servers into requesting URLs

**Application Security** - the world runs on software that must be secure and reliable
- *Purchased Software* - acquired from software vendors for use in many different organizations
- *Developed Software* - custom written to meet the specialized needs of a single organization
- *Application Hardening* - use proper authentication, encrypt sensitive data, validate user input, avoid and remediate known exploits, deploy obfuscation and camouflage
Prompt patching is critical, attackers quickly exploit new vulnerabilities, beware of malicious updates
- *Application Configuration* - type and scope of encryption, users with access to the application, access granted to authorized users, security of underlying infrastructure
	- *Configuration Baselines* - allow quick identification and remediation of security gaps

**Defending Against Directory Traversal** - allows an attacker to manipulate the web server's file structure
- Quick Facts about Unix Filesystems:
	- . references the current directory
	- .. references the directory one level higher in the hierarchy
-  *Directory Traversal Attacks* - when an attacker uses directory navigation references to search for unsecured files on a server

**Race Condition Vulnerabilities** - race conditions are a dangerous application security flaw
- *Race Condition* - occurs when the proper functioning of a security control depends upon the timing of actions performed by the user or computer, uncontrolled race conditions can be significant security vulnerabilities, locks prevent simultaneous transactions from causing race conditions
	- *Time of Check/Time of Use* - time elapsing between authorization and the action