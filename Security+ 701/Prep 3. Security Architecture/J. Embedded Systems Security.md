**Industrial Control Systems**
- *Industrial Control Systems (ICSs)* - monitor and control industry processes
	- ICS Deployments:
		- Building automation systems
		- Workflow automation systems
		- Process automation systems
	- ICSs are Hacker Targets:
		- Attacks have dramatic implications
		- Systems are often not well secured
		- Systems are less likely to be current on patches
	- ICS Types:
		- Supervisory control and data acquisition (SCADA)
		- Distributed control systems (DCSs)
		- Programmable logic controllers (PLCs)
	- *SCADA* - remote monitoring, remote telemetry, reports back to control systems, multiple points of attack
	- *DCS* - focuses on controlling processes, uses sensors and feedback systems, has multiple points of attack
	- *PLC* - handles specialized input and output, ensures uninterrupted processing, connects to a Human Machine Interface
	- *Modbus Protocol* - serial interface communications

**Internet of Things** - the Internet of Things (IoT) is everywhere, smart devices began with a desire for wireless network connectivity
- IoT Security Challenges:
	- Use difficult-to-update software and underlying OS
	- Connect to home and office wireless networks
	- Connect back to cloud services for command and control
- Sensors and Facility Automation:
	- Hospital and medical systems
	- Aircraft and drones
	- Utilities and smart meters

**Securing Smart Devices** - smart devices require regular updates, check for weak default passwords
- *Automatic Updates* - install without the user's knowledge or intervention when published by the device manufacturer
- *Manual Updates* - require that user check for updates and manually download and install them when available
- *Firmware Version Control* - updates applied in orderly fashion
- *Security Wrappers* - vet requests for embedded systems
Use diverse and redundant security controls to protect embedded devices

**Secure Networking for Smart Devices** - smart devices require secure networks, segmenting embedded devices increases network security, network segmentation is the most important control for embedded systems
- *Application Firewalls* - provide added protection for embedded devices
Embedded device security controls are effective for mainframes as well\

**Embedded Systems**
- *Embedded Systems* - technology components of an Internet of Things device that place a full computer inside of another, larger system, printers and multifunction devices contain embedded systems
	- *System on a Chip (SoC)* - combines processing, memory, networking, and other embedded system components on a single chip
	- *Field-programmable Gate Arrays (FPGAs)* - are chips that allow dynamic reprogramming
		- eFUSE technology from IBM allows dynamic modification of the chip
	- *Real-time Operating Systems (RTOSs)* - provide reliable and secure computing for IoT devices
	- *CAN Bus* - facilitates embedded device communications
	- Embedded System Constraints:
		- Power
		- Compute capabilities
		- Network capacity
		- Cryptography
		- Patching
Assess embedded device authentication practices carefully