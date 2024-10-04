**Understanding Authorization** - authorization is the final step in the access control process
- Least Privilege:
	- Limits the potential damage from an insider attack
	- Restricts the ability of an external attacker to leverage a compromised account
- *Separation of Duties* - performing any critical business function should require the involvement of two or more individuals
- *Privilege Creep* - occurs when a user accumulates excess permissions after shifting job responsibilities one or more times
	- *Account Review* - limits privilege creep

**Mandatory Access Controls**
- *Mandatory Access Controls (MAC)* - access control system where the operating system restricts authorizations based upon labels and users are not permitted to modify those authorizations, SELinux provides MAC functionality

**Discretionary Access Controls**
- *Discretionary Access Control (DAC)* - access control system where permissions may be set by the owners of files, computers, and other resources, Windows New Technology File System (NTFS) permissions are an example of a discretionary access control system

**Access Control Lists** - resource owners set DAC permissions through the use of access control lists
- NTFS Permissions:
	- Full control grants complete authority over a resource
	- Read allows the user to read the file
	- Read & Execute also allows the user to execute an application
	- Write allows the user to create files and modify their contents
	- Modify adds the ability to delete files and also includes Read & Execute permissions

**Advanced Authorization Concepts**
- *Implicit Deny* - any action which is not explicitly allowed must be denied
- *RBAC* - in role-based access control systems, permissions are grouped together into functional roles and users are assigned to those roles
- *ABAC* - in attribute-based access control (ABAC) systems, administrators make access control decisions based upon characteristics of the user, object, and environment
- *Location-Based Control* - limits access based upon geographic location
- *Time-of-Day Restriction* - limits access based login time