**Cloud Activities and the Cloud Reference Architecture** - reference architectures provide a useful framework, but they're just a starting point, the ISO cloud reference architecture defines cloud computing activities
- Customer Activities:
	- Use cloud services
	- Perform service trials
	- Monitor services
	- Administer security
	- Provide billing reports
	- Handle problems
	- Administer tenancies
	- Perform business administration
	- Select services
	- Request audit reports
- Provider Activities:
	- Prepare systems and services
	- Monitor services
	- Manage assets
	- Provide audit data
	- Manage customer relationships
	- Perform peering
	- Ensure compliance
	- Provide connectivity
	- Many other activities
- Partner Activities:
	- Design, create, and maintain services
	- Test services
	- Perform audits
	- Set up legal agreements
	- Acquire and assess customers
	- Assess the marketplace

**Cloud Deployment Models** - cloud deployment models describe the cloud environment types that organizations might use
- *Private Cloud* - organization uses a dedicated cloud infrastructure
- *Public Cloud* - organization uses a multitenancy infrastructure, public cloud computing uses a shared responsibility model
- *Hybrid Cloud* - organization uses both private and public cloud
- *Community Cloud* - shared with a consortium
No cloud model is inherently superior to the other approaches, it all depends on the context

*Cloud Service Categories*
- *XaaS* - anything as a service
- *SaaS (Software as a Service)* - customer purchases an entire app, SaaS solutions may be highly specialized such as credit card processing software
- *IaaS (Infrastructure as a Service)* - customer purchases servers/storage
- *PaaS (Platform as a Service)* - customer purchases app platform
- *FaaS (Function as a Service)* - also known as serverless computing


==Customer Responsibilities==
Vendor Responsibilities

| IaaS            | PaaS            | SaaS        |
| --------------- | --------------- | ----------- |
| ==Data==        | ==Data==        | ==Data==    |
| ==Application== | ==Application== | Application |
| ==OS==          | OS              | OS          |
| Hardware        | Hardware        | Hardware    |
| Data Center     | Data Center     | Data Center |

**Security and Privacy Concerns in the Cloud**
- *Privacy* - protects the confidentiality rights of individuals whose information we store, process, or transmit
Governance ensures effective oversight of cloud use in an organization, regular audits verify cloud service providers are fulfilling their security and operational obligations, cloud providers serving regulated customers must support compliance efforts

**Data Sovereignty** - organizations spread their data across a variety of cloud providers, cloud providers spread data across multiple geographic regions
- *Data Sovereignty* - local laws apply to data
Data is only subject to laws of the jurisdictions where it is collected, stored, or processed, storing data in multiple locations subjects it to multiple jurisdictions
- Data Sovereignty Controls:
	- Determine where cloud providers will store data
	- Put storage locations in writing
	- Use encryption to protect data

**Operational Concerns in the Cloud** - cloud computing raises new operational concerns
- *Availability* - how much uptime is required?
- *Resiliency* - how many failures are tolerable?
- *Performance* - how much demand can be handled?
- *SLAs (Service Level Agreements)* - document vendor obligations
IT teams must coordinate internal maintenance schedules, cloud maintenance schedules, and business requirements
- *Reversibility* - can we roll back operations to the original state prior to a cloud transition?
- *Portability* - can we move workloads between cloud vendors?
- *Interoperability* - will our cloud solutions from different vendors work together?