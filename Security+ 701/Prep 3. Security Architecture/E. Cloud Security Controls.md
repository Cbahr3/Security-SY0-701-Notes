**Cloud Firewall Considerations** - network security groups work at the same layers of the OSI model as network firewalls, cloud service providers do maintain firewalls but customers can't modify them directly
- *Network Security Groups* - serve as IaaS firewalls, maintaining network security groups is a customer responsibility

**Cloud Application Security** - building secure cloud applications requires the integration of many different services, on-premises security controls often map directly to cloud controls
- *Firewall* - controls network access
- *Transport Layer Security* - encrypts data in transit
- *Full Disk Encryption* - encrypts data at rest
- *Application Virtualization* - centralizes sensitive data
- *Secure Web Gateway* - filters web traffic
Defense in depth requires the use of overlapping security controls

**Cloud Provider Security Controls**
- *Cloud-Native Controls* - security controls offered by cloud providers that tightly integrate with the provider's service offerings
- *Third-Party Controls* - security controls offered third-party vendors that integrate with cloud providers through their API and may work across multiple cloud platforms
- *Resource Policy* - limits cloud service usage
- *Transit Gateway* - links on-premises and cloud networks
- *Secret Management* - protects keys and other credentials