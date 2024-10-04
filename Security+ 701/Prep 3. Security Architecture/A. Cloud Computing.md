**What is the Cloud?** - cloud computing is transforming information technology across industries
- *Cloud Computing* - delivering computing resources to a remote customer over a network, accessing web-based email is cloud computing, building servers in AWS is cloud computing
	- *Cloud Computing (NIST Definition)* - ubiquitous, convienient, on-demand network access to a shared pool of configurable computing resources (e.g., networks, servers, storage, applications, and services), rapidly provisioned and released, minimal management effort or service provider interaction

**Cloud Computing Roles** - people and organizations play different roles in the world of cloud computing
- *Cloud Service Provider* - offers cloud computing services for sale the third parties
- *Cloud Customer* - purchases cloud computing services from one or more cloud service providers
- *Cloud Service Partner* - provides add-on services
- *CASB (Cloud Access Security Broker)* - provides IAM (Identity & Access Management) services

**Drivers for Cloud Computing**
- *On-Demand Self-Service* - available when you need it
- *Scalability* - increasing capacity with demand
	- *Horizontal Scaling* - adds more servers to the pool to meet increased demand
	- *Vertical Scaling* - adds more resources (for example, CPU or memory) to existing servers to meet increased demand
- *Elasticity* - expanding and contracting quickly
- *Broad Network Access* - anytime, anywhere access
- *Measured Service* - paying only for what you consume

**Multitenant Computing**
- *Multitenancy* - shared computing resources
- *Isolation* - users don't impact each other
- *Oversubscription* - sold capacity exceeds actual capacity
- *Resource Pooling* - CPU and memory shared among users
When isolation breaks down, performance suffers

**Cloud Considerations**
- *Cost-Benefit Analysis* - is the cloud worth it?
	- On-Premises Cost vs. Cloud Cost
		- Cost Factors at Scale:
			- Electricity costs
			- Data center facility rental/acquisition/maintenance
			- Training costs
			- Consulting services
			- Staff time
		- Intangible Benefits:
			- Ease of deployment
			- Risk transference
			- Availability
			- Resilience and ease of recovery
			- Responsiveness
			- Scalability and elasticity
			- Emerging technolgies
			- CapEx vs OpEx
			- Fun

**Security Service Providers**
- *MSPs (Managed Service Providers)* - offer information technology services to customers
	- *MSSPs (Managed Security Service Providers)* - provide security services for other organizations as a managed service, MSSPs must be carefully monitored, MSSPs may also be referred to as SECaaS (Security as a Service)
		- MSSP Service Examples:
			- Manage an entire security infrastructure
			- Monitor system logs
			- Manage firewalls or networks
			- Perform identity and access management
		- *CASBs (Cloud Access Security Brokers)* - add a third-party security layer to the interactions that users have with other cloud services
			- *Network-Based CASB* - broker intercepts traffic between the user and the cloud service, monitoring for security issues, broker can block requests
			- *API-Based CASB* - the broker queries the cloud service via API, broker may not be able to block requests, depending upon API capabilities
MSSP relationships should be carefully documented