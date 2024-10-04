**Virtualization** - mainframes dominated data centers of past decades, the client/server model emerged in the 1980s and 1990s, now most data centers leverage virtualization technology
- *Virtualization* - host machines run on physical hardware, host machines provide services to several virtualized guest machines, the hypervisor tricks each guest into thinking it is running on dedicated hardware
	- *Type 1 Hypervisor* - hypervisor runs directly on top of the hardware and then hosts guest operating systems on top of that. most common form of virtualization found in data centers
	- *Type 2 Hypervisor* - the physical machine runs an operating system of its own and the hypervisor runs as a program on top of that operating system
	- Virtualization Security:
		- Virtual machine isolation is critical
		- Each server must have access to only its own memory and storage
		- VM escape attacks attempt to break out of the guest environment
Virtualization platforms must be patched against security vulnerabilities
- *VM Sprawl* - unused and unmaintained servers

**Desktop and Application Virtualization**
- *(VDI) Virtual Desktop Infrastructure* - provides network-based access to a desktop computing environment
- *Application Virtualization* - streams applications to the user's desktop
Desktop and application virtualization enable the use of thin client devices