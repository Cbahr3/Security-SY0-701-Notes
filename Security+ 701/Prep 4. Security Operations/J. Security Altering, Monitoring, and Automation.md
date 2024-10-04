**Logging Security Information** - system monitoring creates massive amounts of information
- Log and Data Sources:
	- Network or NetFlow
	- DNS
	- System
	- Application
	- Authentication
	- VoIP
	- Dump files
	- Vulnerability scans
- *Syslog* - provides a logging standard, Linux supports syslog natively
	- Syslog Message Components:
		- Header (timestamp, source address)
		- Facility (source of the message on the sending system)
		- Severity (importance value from 0 to 7)
		- Message (details of the situation)
	- Syslog Versions:
		- Syslog is the original standard and is rarely used today
		- syslog-ng added security and delivery enhancements in 1998
		- Rsyslog added further enhancements in 2004
		- journalctl uses a binary journal format
Log retention must balance security and cost
- *Tags* - facilitate searching, filtering, and analysis
- *NXLog* - centralizes the management of disparate logs

**Security Information and Event Management** - systems generate far too many log records for manual analysis, artificial intelligence (AI) can help solve security data overload
- SIEM:
	- Central, secure collection point for logs
		- All systems send log entries directly to the SIEM
	- Source of artificial intelligence
		- SIEMs detect patterns that other systems might miss
	SIEMs have access to log entries from across the organization
- *Intrusion Detection System* - triggers the initial alert
- SIEM Dashboards:
	- Provide a centralized view of security information
	- Generate alerts for unusual activity
	- Facilitate trend analysis
	- Offer adjustable sensitivity
- *Security Orchestration, Automation, and Response (SOAR)* - enhanced versions of SIEMs
	- *Playbooks* - process-focused responses to security events, including both human and automated actions
	- *Runbooks* - automated responses to security events that execute immediately and aid human investigators

**Monitoring Activities**
- *Monitoring* - observing activity for anomalies
- *Alerting* - notifying personnel of anomalies
- *Scanning* - automatically seeking vulnerabilities
- *Reporting* - provides insight into data
- *Quarantine* - isolates a potentially infected system from the rest of the network to prevent the spread of harm
- *Alert Tuning* - adjusts the alerting system to reduce the rate of false positive alerts
Effective monitoring includes response and remediation activities

**Endpoint Monitoring** - many endpoints connect to our networks, a single device can serve as the jumping-off point for a broader attack, monitor processor, memory, and file system activity, security tools provide important insight into endpoint behavior, behavior monitoring can detect specific exploit techniques
- *User and Entity Behavior Analytics (UEBA)* - compares user activity to individual baselines

**Automation and Orchestration** - standardizing tasks helps you identify automation opportunities, SOAR platforms offer opportunities to improve your use of threat intelligence
- *Scripting* - automates tasks with code
	- Scripting Use Cases:
		- User provisioning
		- Resource provisioning
		- Guardrails
		- Security groups
		- Ticket creation
		- Escalation
		- Enabling/disabling services and access
		- Continuous integration and testing
		- Integrations and APIs
	- Scripting Benefits:
		- Efficiency/time saving
		- Enforcing baselines
		- Standard infrastructure configurations
		- Scaling in a secure manner
		- Employee retention
		- Reaction time
		- Workplace multiplier
	- Scripting Considerations:
		- Complexity
		- Cost
		- Single point of failure
		- Technical debt
		- Ongoing supportability