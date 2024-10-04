**Introduction to Forensics** - security professionals engage in digital forensics
- *Digital Forensics* - investigative techniques that collect, preserve, analyze, and interpret digital evidence
Investigations must never alter evidence
- *Volatility* - the relative permanence of a piece of evidence; evidence that may not last long is more volatile than more permanent sources of evidence
	- Order of Volatility:
		1. Network traffic
		2. Memory contents
		3. System and process data
		4. Files
		5. Logs
		6. Archived records
Time offsets help correlate records from different sources
- Consider Alternate Evidence Sources:
	- Video recordings
	- Witness statements
Track your use of time and resources

**System and File Forensics** - digital evidence requires digital forensic techniques
- *Images* - take the place of original physical media
- *Write Blockers* - also known as forensic disk controllers, prevent accidental modification of disks during imaging
Hashes protect evidence, they provide a unique file signature, use hashes to demonstrate that a file hasn't been altered, digital signatures provide non-repudiation
- *File Metadata* - contains a wealth of forensic information
- Other Forensic Sources:
	- Screenshots
	- Memory contents
	- Process table
	- Operating system configuration
Never try to perform forensics yourself unless you've received appropriate training

**Chain of Custody**
- *Chain of Custody* - provides a paper trail of evidence
Evidence should be labeled and stored in a sealed evidence container
- Evidence Log Events:
	- Initial collection
	- Transfer
	- Storage
	- Opening and resealing the container
- Evidence Log Entry Details:
	- Investigator name
	- Date and time
	- Purpose
	- Nature of action
Evidence logs must be available to present in court

**E-Discovery and Evidence Production** - cybersecurity professionals often assist with electronic discovery efforts
- There are three major steps in the electronic discovery process:
	- *Preservation* - legal holds require the preservation of relevant electronic and paper records, system administrators must suspend the automatic deletion of relevant logs
	- *Collection* - security teams often assist in collection efforts, electronic discovery management systems coordinate collection efforts
		- Sources of Electronic Records:
			- File servers
			- Endpoint systems
			- Email messages
			- Enterprise systems and cloud services
	- *Production* - if production occurs, attorneys must review documents for relevance and turn them over to the other side, most litigation holds never move forward to the production phase

**Investigation Data Sources** - cybersecurity investigators are digital detectives
- Logs Provide Valuable Evidence:
	- Firewall logs
	- Application logs
	- Endpoint logs
	- OS-specific security logs
	- IDS/IPS logs
	- Network logs
- Other Data Sources:
	- Metadata
	- Vulnerability scans
	- Automated reports
	- Dashboards
	- Packet captures