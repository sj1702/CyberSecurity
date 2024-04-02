Network Design
The objective of network design is to satisfy data communication requirements and result in efficient overall performance.

Several elements that are considered when planning for security in a network are: 

	- Network Segmentation:
	Network segmentation involves controlling traffic among networked devices. Complete or physical network segmentation occurs when a network is isolated from all outside communications, so transactions can only occur between devices within the segmented network.
	
	- Demilitarized Zone:
	A DMZ is a network area that is designed to be accessed by outside visitors but is still isolated from the private network of the organization. The DMZ is often the host of public web, email, file and other resource servers.
	
	- Virtual Local Area Network:
	VLANs are created by switches to logically segment a network without altering its physical topology.
	
	- Virtual Private Network:
	A virtual private network (VPN) is a communication tunnel that provides point-to-point transmission of both authentication and data traffic over an untrusted network.
	
	- Defense in Depth:
	Defense in depth uses multiple types of access controls in literal or theoretical layers to help an organization avoid a monolithic security stance.
	
	- Network Access Control:
	Network access control (NAC) is a concept of controlling access to an environment through strict adherence to and implementation of security policy.
	
	
	
	
Defense in Depth:
Defense in depth uses a layered approach when designing the security posture of an organization. Think about a castle that holds the crown jewels. The jewels will be placed in a vaulted chamber in a central location guarded by security guards. The castle is built around the vault with additional layers of security—soldiers, walls, a moat. The same approach is true when designing the logical security of a facility or system. Using layers of security will deter many attackers and encourage them to focus on other, easier targets. 

Defense in depth provides more of a starting point for considering all types of controls—administrative, technological, and physical—that empower insiders and operators to work together to protect their organization and its systems. 

Here are some examples that further explain the concept of defense in depth: 

	-Data: Controls that protect the actual data with technologies such as encryption, data leak prevention, identity and access management and data controls.
	-Application: Controls that protect the application itself with technologies such as data leak prevention, application firewalls and database monitors.
	-Host: Every control that is placed at the endpoint level, such as antivirus, endpoint firewall, configuration and patch management.
	-Internal network: Controls that are in place to protect uncontrolled data flow and user access across the organizational network. Relevant technologies include intrusion detection systems, intrusion prevention systems, internal firewalls and network access controls.
	-Perimeter: Controls that protect against unauthorized access to the network. This level includes the use of technologies such as gateway firewalls, honeypots, malware analysis and secure demilitarized zones (DMZs).
	-Physical: Controls that provide a physical barrier, such as locks, walls or access control.
	-Policies, procedures and awareness: Administrative controls that reduce insider threats (intentional and unintentional) and identify risks as soon as they appear. 
	
	
Data are on Servers; Servers are in Data Centers; which are secured with Trusted Software by Trusted System Administrators; which are secured by Applications used by Standards and best Practices, ethical penetration testers and threat actors; which are secured by Hosts who are Trusted Developers with Trusted Update/ Lifecycle Process; which are secured by trusted LAN Network Systems; which are secured by Perimeter Network used by Trusted Web Apps and Trusted Internal Users having training and awareness with Policy and Procedures; which are secured by Physical Perimeter through Trusted Public-facing People Processes and Facilities Security.