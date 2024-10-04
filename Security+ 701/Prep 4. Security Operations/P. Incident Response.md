**Build an Incident Response Program**
- *Incident Response Plan* - provides structure during cybersecurity incidents, incident response plans describe the policies and procedures governing cybersecurity incidents, prior planning leads to strong incident response, failure to conduct advance planning may lead to disaster
	- Incident Response Plan Elements:
		- Statement of purpose
		- Strategies and goals for incident response
		- Approach to incident response
		- Communication with other groups
		- Senior leadership approval
Consult NIST SP 800-61 as you develop your plan

**Incident Identification** - maintain a watchful eye for security incidents, monitoring is crucial to effective incident identification, the first reports of an incident may come from external sources, first responders must act quickly, isolate affected systems, the highest priority of a first responder must be containing through isolation, strategic intelligence programs facilitate incident identification efforts, counterintelligence hinders adversary abilities to gather intelligence

**Escalation and Notification** - after initial containment efforts, move into escalation and notification mode
- Escalation and Notification Objectives:
	- Evaluate incident severity based upon impact
	- Escalate response to an appropriate level
	- Notify management and other stakeholders
- Triaging Incidents:
	- Low-Impact Incidents:
		- Have minimal potential to affect security
		- Are normally handled by first responders
		- Don't require after hours response
	- Moderate-Impact Incidents:
		- Have significant potential to affect security
		- Trigger incident response team activation
		- Require prompt notification to management
	- High-Impact Incidents:
		- May cause critical damage to information or systems
		- Justify an immediate, full response
		- Require immediate notification to senior management
		- Demand full mobilization of incident response team
First responders must have the ability to quickly activate a full incident response process

**Mitigation** - control damage and loss to the organization through containment
- Containment Strategy Evaluation:
	1. Damage potential
	2. Evidence preservation
	3. Service availability
	4. Resource requirements
	5. Expected effectiveness
	6. Solution time frame
Balance business needs and security objectives, attackers may detect containment actions. mitigation ends with stability, business functioning without danger

**Containment Techniques** - the first hours of an incident response are stressful
- *Containment* - limits the damage
	- *Segmentation* - separate to quarantine VLAN
	- *Isolation* - send to own quarantine network
	- *Removal* - remove from network

**Incident Eradication and Recovery**
- *Eradication* - removes all traces of an incident
- *Recovery* - restore normal operations
Eradication and recovery activities are closely linked, attackers compromise systems, rebuild any affected systems to avoid future issues, correct the security issues that led to the incident in the first place
- Endpoint Security Practices:
	- Application whitelisting
	- Application blacklisting
	- Quarantine
	- Access controls
- Enterprise Security Controls:
	- Firewall rules
	- Mobile device management (MDM)
	- Data loss prevention (DLP)
	- URL and content filtering
	- Update or revoke digital certificates
Sanitization and secure disposal prevents confidential information leakage
- Sanitization Techniques:
	- *Clearing* - overwrites sensitive information to frustrate casual analysis
	- *Purging* - uses more advanced techniques to frustrate laboratory analysis
	- *Destroying* - completely obliterates the media through shredding, pulverization, melting, or burning
Use the NIST flow chart to select an appropriate sanitization technique

**Post-Incident Activities**
- Post-Incident Activities:
	- *Lessons learned* - provides incident responders with an opportunity to reflect on the incident response efforts and offer feedback that will improve the organization's response to future incidents, use a trained facilitator, time is of the essence, create a report that includes lessons learned and recommendations, follow your change management process
		- Lessons Learned Questions:
			- Exactly what happened, and at what times?
			- How well did staff and management perform?
			- Were documented procedures followed?
			- Were those procedures adequate?
			- What information was needed sooner?
			- Did any actions inhibit the recovery effort?
			- What would staff and management do differently next time?
			- How could information sharing improve?
			- What could prevent similar incidents?
			- What should the organization watch for?
			- What tools or resources are needed?
		- *Incident Summary Report* - describes response efforts, include a root cause analysis in the report
	- *Evidence retention* - retain any evidence necessary to comply with company policy and legal requirements
	- *Indicator-of-compromise generation* - incorporate new indicators of compromise in your security monitoring program
	- *Root cause analysis* - include a root cause analysis in the report

**Incident Response Training and Testing** - train your incident response team to keep skills sharp, tabletop exercises gather the team together, simulations use a specific scenario to test incident response, simulations may become hands-on penetration tests