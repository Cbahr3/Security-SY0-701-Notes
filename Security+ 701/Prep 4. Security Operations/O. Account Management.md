**Understanding Account and Privilege Management**
- Account Management Tasks:
	- Implement least privilege
	- Implement separation of duties
	- Implement job rotation
	- Manage the account life cycle
- *Job Rotation* - regularly move people between jobs to prevent fraud
- *Mandatory Vacation* - enforce periods of time when employees have no access to systems
Standard naming conventions facilitate user identification

**Privileged Access Management** - privilege access management solutions safeguard administrative accounts
- *Password Vaulting* - stores administrative passwords
- *Command Proxying* - eliminates the need for direct server access
- *Monitoring* - logs administrative user activity
- *Credential Management* - rotates passwords and access keys
Privileged account management solutions should provide an emergency access workflow, only use privileged accounts when necessary
- *Ephemeral Accounts* - grant temporary access
Limit access to sudo privileges

**Provisioning and Deprovisioning** - provisioning and deprovisioning accounts is a critical identity and access management task
- *Provisioning* - after onboarding, administrators create authentication credentials and grant appropriate authorization
- *Deprovisioning* - during the offboarding process, administrators disable accounts and revoke authorizations at the appropriate time
	- Prompt Termination Is Critical:
		- Prevents users from accessing resources without permission
		- Is especially critical when a user leaves under adverse circumstances
	- *Routine Workflow* - disables accounts on a scheduled basis for planned departures
	- *Emergency Workflow* - immediately suspends access when user is unexpectedly terminated
		- Incorrectly Timed Account Revocations:
			- May inform a user in advance of pending termination
			- May allow a user access to resources after termination