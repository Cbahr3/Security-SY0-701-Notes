**Business Continuity Planning**
- *Business Continuity Planning (BCP)* - the set of controls designed to keep a business running in the face of adversity, whether natural or man-made, also known as continuity of operations planning (COOP)
	- Defining the BCP Scope:
		- What business activities will the plan cover?
		- What systems will it cover?
		- What controls will it consider?
- *Business Impact Assessment (BIA)* - identifies and prioritizes risks
Business continuity planning in the cloud is a partnership between providers and customers

**Business Continuity Controls** - redundancy protects against failure of a single component
- *Single Point of Failure Analysis* - identifies and removes SPOFs, SPOF analysis continues until the cost of addressing risks outweighs the benefit
- IT Contingency Scenario Examples:
	- Sudden bankruptcy of a key vendor
	- Insufficient storage or compute capacity
	- Failure of utility service
Remember to perform succession planning for staff as well

**High Availability and Fault Tolerance**
- *High Availability* - uses multiple systems to protect against service failure
- *Fault Tolerance* - makes a single system resilient against technical failure
- *Power Supplies* - contain moving parts, have high failure rates, can be redundant, may use multiple power sources
	- *Uninterruptible Power Supplies (UPSs)* - supply battery power to devices during brief disruptions
	- *Managed Power Distribution Units (PDUs)* - provide power cleaning and management for a rack
	- *Redundant Array of Inexpensive Disks (RAID)*:
		- Disk mirroring, RAID 1, stores the same data on two different disks
		- Disk striping, with parity, RAID 5, uses three or more disks to store data and parity information
		RAID is a fault tolerance technique, not a backup strategy
- Network Redundancy:
	- Multiple internet service providers
	- NIC teaming
	- Multipath networking (especially for storage)
- Platform Diversity:
	- Technologies
	- Vendors
	- Cryptography
	- Security controls
- *Multicloud* - adds resilience to operations

**Disaster Recovery** - business continuity plans sometimes fail
- *Disaster Recovery* - disaster recovery capabilities are designed to restore a business to normal operations as quickly as possible, disaster recovery is a subset of business continuity, disasters may come from internal or external sources
	- Initial Response:
		- Contain the damage caused by the disaster
		- Recover whatever capabilities may be immediately restored
		- Include a variety of activities depending upon the nature of the disaster
	Employee responsibilities will change dramatically during disaster recovery
	- Disaster Communications:
		- Initial activation of the disaster recovery team
		- Regular status updates
		- Tactical communications
	After the danger passes, the team shifts to assessment mode
	- Disaster Recovery Metrics:
		- The *recovery time objective (RTO)* is the maximum amount of time that it should take to recover a service after a disaster
		- The *recovery point objective (RPO)* is the maximum time period from which data may be lost in the wake of a disaster
		- The *recovery service level (RSL)* is the percentage of a service that must be available during a disaster
	After developing a plan, responders restore services in an orderly fashion, disaster recovery efforts end only when the business is operating normally in its primary environment, team members should receive regular training on their disaster recovery responsibilities

**Backups** - the loss of critical business data can have catastrophic effects
- *Backups* - provide a data safety net
	- Backup Media:
		- Tape backups
		- Disk-to-disk backups
		- Cloud backups
	- *Full Backup* - includes a complete copy of all data, snapshots and images are types of full backups
	- *Differential Backup* - includes all data modified since the last full backup
	- *Incremental Backup* - includes all data modified since the last full or incremental backup
	- *Journaling* - records a transaction log of changes
Select your backup frequency to balance the time and cost of performing backups with the potential for data loss, encrypt backups to protect against the loss of sensitive data

**Restoring Backups** - we often restore backups in response to small-scale situations, for large-scale recovery efforts, the order of restoration is important, organizations should prioritize the recovery of critical assets
- *Non-persistence* - allows us to back up only unique data
Configuration problems may be corrected by reverting to a known state, live boot media may allow recovery of data from a device with a corrupted operating system

**Disaster Recovery Sites**
- *Disaster Recovery Sites* - provide alternative data processing
	- *Hot Sites* - fully operational data centers, stocked with equipment and data, available at a moment's notice, very expensive
	- *Cold Sites* - empty data centers, stocked with core equipment, network, and environmental controls, relatively inexpensive, operational in weeks or months
	- *Warm Sites* - stocked with all necessary equipment and data, not maintained in a parallel fashion, similar in expense to hot sites, available in hours or days
	- *Offsite Storage* - geographically dispersed, site resiliency, manual transfer or site replication through SAN or VM, online or offline backups
Consider integrating alternative business processes into your disaster recovery plan

**Testing BC/DR Plans**
- Disaster Recovery Testing Goals:
	- Validate that the plan functions correctly
	- Identify necessary plan updates
- Disaster Recovery Test Types:
	- *Tabletop Exercises* - gather the team together for a formal review of the disaster recovery plan
	- *Simulations* - use a practice scenario to test the disaster recovery plan
	- *Parallel Processing Tests* - activate the disaster recovery environment but do not switch operations there
	- *Failover Tests* - switch primary operations to the alternative environment and can be very disruptive to business
	Testing strategies often combine multiple types of tests

**Capacity Planning**
- *Capacity Planning* - allows organizations to anticipate and adapt to future demand, technology system must be robust and scalable, infrastructure must incorporate redundancy and reliability, people should be strong, adaptable, and cross-trained