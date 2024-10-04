**Cloud Compute Resources** - virtualized servers run in cloud data centers
- *High Availability* - uses resources across zones
- *Instance Awareness* - reduces VM sprawl

**Cloud Storage** - storage is a fundamental building block of cloud computing
- *Block Storage* - allocates a large chunk of storage for access as a disk volume managed by the operating system, magnetic, solid state
- *Object Storage* - stores files as individual objects managed by the cloud service provider, high availability, archival
Most enterprise computing environments have a need for both block and object storage
- Cloud Storage Costs:
	- Object storage is much less expensive than block storage in the cloud
	- Object storage costs are incurred only when used, while block storage must be allocated and paid for in drive-sized blocks
- Cloud Storage Security:
	- Set permissions properly
	- Make use of encryption for sensitive data
	- Replicate data to multiple data centers

**Cloud Networking** - cloud customers must build and manage virtual networks in the cloud, cloud networking is highly virtualized and customizable, in a traditional data center, VLANs (Virtual LANs) separate systems of differing security levels, cloud providers use VPCs (Virtual Private Clouds) and similar concepts for the same purpose
- *VPC Endpoints* - provide secure VPC interconnection
- *SDN* - software-defined networking
- *SDV* - software-defined visibility

**Cloud Databases** - the cloud provides many database hosting options
- Cloud Database Options:
	1. Build databases on virtualized servers
		- Requires spinning up a server and installing/configuring databases
		- Resembles on-premises operations
		- Requires customer management of servers and databases
	2. Use a managed database server
		-  Request database from cloud provider using platform of choice
		-  Transfer maintenance responsibility to the cloud provider
		-  Incurs additional costs
	3. Use a cloud-native database platform
		- Allows use of relational databases, key-value stores, graph databases, and other options
		- Offers high degree of cloud optimization
		- Requires retooling existing applications

**Cloud Orchestration** - hybrid environments add complexity to cloud operations
- *Cloud Orchestration* - automates cloud management
- *Infrastructure as Code* - manages cloud programmatically
Cloud orchestration solutions access resources through the vendor's API, cloud providers and third-party vendors both offer orchestration solutions

**Containers**
- *Containers* - lightweight application virtualization, containers are a lightweight alternative to virtual servers, contain application code and dependencies only, run on containerization platforms, use the host's operating system
Isolation is the most critical container security issue

**SOA and microservices**
- *SOA (Service-Oriented Architecture)* - design philosophy that embraces the use of discrete services that may be accessed by customers in a black-box fashion
	- Service Characteristics:
		- Logical representations of a repeatable business activity with a specified outcome
		- Self-contained
		- May be composed of other services
		- Black-box nature
Service-oriented architectures facilitate the integration of services from different vendors
- *Microservices* - fine-grained services