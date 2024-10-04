**Authentication Factors**
- Authentication Factors:
	- Something you know
	- Something you are
	- Something you have
	- Somewhere you are
- *False Acceptance* - system misidentifies an individual as an authorized user, measured by the false acceptance rate (FAR)
- *False Rejection* - system fails to recognize an authorized user, measured by the false rejection rate (FRR)
FAR and FRR are not good measures on their own, Crossover Error Rate (CER) or the intersection of FAR and FRR

**Multifactor Authentication** - authentication mechanisms can be tricked
- *Multifactor Authentication* - combines authentication techniques from two or more of the authentication categories: something you know, something you have, something you are, and somewhere you are

**Something You Have** - push notifications allow you to acknowledge a login attempt through a smartphone app, SMS and phone-based authentication mechanisms provide weak security, static codes provide a backup to multifactor authentication

**Password Policy** - passwords remain the most common authentication mechanism, passwords should be at least eight characters long, passwords may be composed of uppercase and lowercase letters, digits, and symbols, current NIST guidance says that complex passwords should be allowed, but not required, password expiration policies prevent extended use of compromised passwords by an attacker, current NIST guidance says that passwords should not expire
- *Lockout Policies* - lock out accounts after many incorrect login attempts
- *Disablement* - disable unused accounts
- Password Recovery Mechanisms:
	- Allow users to reset passwords on a self-service basis
	- Relieve burden on help desk
	- Improve user satisfaction with IT

**Password Managers** - it's important to use strong, unique passwords on every website you visit, but this can be challenging
- *Password Managers* - securely store, manage, and retrieve passwords
	- Benefits of Password Managers:
		- Promote the use of strong passwords
		- Reduce the risk of phishing attacks
		- Use strong encryption to protect passwords
		- Sync across devices
		- Store other information securely
Choose a passwords manager you can trust

**Passwordless Authentication** - passwords are clunky and inconvenient, passworldess authentication improves the user experience by moving away from passwords
- Passwordless Authentication Benefits:
	- Phishing resistance
	- Simplicity for users
	- Reduced management overhead
	- Physical control of authentication objects
- Passwordless Challenges:
	- Account lockout
	- Cost of security keys

**Single Sign-On and Federation**
- *Federation and Single Sign-On* - seek to reduce the burden of identity and access management
	- Federated Identity Management:
		- Individuals may have accounts across multiple systems
		- Federated identity management systems share identity information
		- This reduces the number of individual identities a user must have
	- *Single Sign-On (SSO)* - authentication system that shares a single authentication session across multiple systems, avoiding asking users to log in multiple times, SSO presents users with a single login screen and creates a session that persists across other systems

**Kerberos and LDAP**
- *Kerberos* - is one of the core protocols for Microsoft Active Directory, ticket-based authentication system that allows users to authenticate to a centralized service and then use tickets to gain access to distributed services
- *LDAP* - the Lightweight Access Protocol (LDAP) provides the means to query a centralized directory service, such as Microsoft Active Directory
- TCP Ports:
	- Kerberos uses port 88
	- LDAP uses port 389
	- Secure LDAP uses port 636
- NTLM Authentication:
	- NT LAN Manager
	- Was widely used on Windows systems for many years
	- Depends upon a hash-based challenge-response protocol
	- NTLM Security Issues:
		- Weak encryption
			- Jeopardizes the security of encrypted hash values
		- Pass the hash
			- Allows the use of credentials from one system to gain access to another system
	Avoid the use of NTLM

**SAML**
- *SAML* - the Security Assertion Markup Language (SAML) allows single sign-on (SSO) within a web browser across a variety of systems

**OAuth and OpenID Connect** - OAuth and OpenID Connect are related protocols, OAuth is an authorization protocol, OpenID Connect is an authentication protocol

**Certificate-based Authentication** - digital certificates may be used for authentication, certificates contain a signed copy of a public key, certificate authorities create digital certificates for public keys used in authentication
- Certificate Authentication Uses:
	- SSH connections
	- Smart cards (CAC/PIV)
	- Network access (802.1x)