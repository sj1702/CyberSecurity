## Preventing Threats:
While there is no single step you can take to protect against all threats, there are some basic steps you can take that help reduce the risk of many types of threats.

Keep systems and applications up to date. Vendors regularly release patches to correct bugs and security flaws, but these only help when they are applied. Patch management ensures that systems and applications are kept up to date with relevant patches. 
Remove or disable unneeded services and protocols. If a system doesn’t need a service or protocol, it should not be running. Attackers cannot exploit a vulnerability in a service or protocol that isn’t running on a system. As an extreme contrast, imagine a web server is running every available service and protocol. It is vulnerable to potential attacks on any of these services and protocols. 
Use intrusion detection and prevention systems. As discussed, intrusion detection and prevention systems observe activity, attempt to detect threats and provide alerts. They can often block or stop attacks.  
Use up-to-date anti-malware software. We have already covered the various types of malicious code such as viruses and worms. A primary countermeasure is anti-malware software.  
Use firewalls. Firewalls can prevent many different types of threats. Network-based firewalls protect entire networks, and host-based firewalls protect individual systems. This chapter included a section describing how firewalls can prevent attacks. 




Antivirus:

The use of antivirus products is strongly encouraged as a security best practice and is a requirement for compliance with the Payment Card Industry Data Security Standard (PCI DSS). There are several antivirus products available, and many can be deployed as part of an enterprise solution that integrates with several other security products.

Antivirus systems try to identify malware based on the signature of known malware or by detecting abnormal activity on a system. This identification is done with various types of scanners, pattern recognition and advanced machine learning algorithms.

Anti-malware now goes beyond just virus protection as modern solutions try to provide a more holistic approach detecting rootkits, ransomware and spyware. Many endpoint solutions also include software firewalls and IDS or IPS systems.



Scans:

Here is an example scan from Zenmap showing open ports on a host.

	Scanning 6 hosts [1000 ports/host]
	Discovered open port 143/tcp on 172.20.1.131
	Discovered open port 80/tcp on 172.20.1.129
	Discovered open port 22/tcp on 172.20.1.132
	Discovered open port 22/tcp on 172.20.1.129
	Discovered open port 135/tcp on 172.20.1.131
	Discovered open port 80/tcp on 172.20.1.131
	Discovered open port 22/tcp on 172.20.1.131
	Discovered open port 3306/tcp on 172.20.1.131
	Discovered open port 443/tcp on 172.20.1.131
	Discovered open port 445/tcp on 172.20.1.131
	Discovered open port 110/tcp on 172.20.1.131
	Discovered open port 139/tcp on 172.20.1.131
	Discovered open port 80/tcp on 172.20.1.127
	Discovered open port 25/tcp on 172.20.1.131
	Discovered open port 21/tcp on 172.20.1.131
	Discovered open port 22/tcp on 172.20.1.127
	Discovered open port 49153/tcp on 172.20.1.131
	Discovered open port 49154/tcp on 172.20.1.131
	Discovered open port 443/tcp on 172.20.1.127

Regular vulnerability and port scans are a good way to evaluate the effectiveness of security controls used within an organization. They may reveal areas where patches or security settings are insufficient, where new vulnerabilities have developed or become exposed, and where security policies are either ineffective or not being followed. Attackers can exploit any of these vulnerabilities.





Firewalls:

In building construction or vehicle design, a firewall is a specially built physical barrier that prevents the spread of fire from one area of the structure to another or from one compartment of a vehicle to another. Early computer security engineers borrowed that name for the devices and services that isolate network segments from each other, as a security measure. As a result, firewalling refers to the process of designing, using or operating different processes in ways that isolate high-risk activities from lower-risk ones.

Firewalls enforce policies by filtering network traffic based on a set of rules. While a firewall should always be placed at internet gateways, other internal network considerations and conditions determine where a firewall would be employed, such as network zoning or segregation of different levels of sensitivity. Firewalls have rapidly evolved over time to provide enhanced security capabilities. This growth in capabilities can be seen in the graphic below, which contrasts an oversimplified view of traditional and next-generation firewalls. It integrates a variety of threat management capabilities into a single framework, including proxy services, intrusion prevention services (IPS) and tight integration with the identity and access management (IAM) environment to ensure only authorized users are permitted to pass traffic across the infrastructure. While firewalls can manage traffic at Layers 2 (MAC addresses), 3 (IP ranges) and 7 (application programming interface (API) and application firewalls), the traditional implementation has been to control traffic at Layer 4.

 - Traditional Firewalls:
		Firewall PORTS IP Address:: IDS IPS, Web Proxy, Antivirus Gateway, VPN
		
 - Next-Generation Firewalls: (IAM, Attributes)
		Firewall PORTS IP Address:: IDS IPS, Web OProxy, Anti-bot, Antivirus Gateway, VPN, FaaS


Intrusion Prevention System (IPS):

An intrusion prevention system (IPS) is a special type of active IDS that automatically attempts to detect and block attacks before they reach target systems. A distinguishing difference between an IDS and an IPS is that the IPS is placed in line with the traffic. In other words, all traffic must pass through the IPS and the IPS can choose what traffic to forward and what traffic to block after analyzing it. This allows the IPS to prevent an attack from reaching a target. Since IPS systems are most effective at preventing network-based attacks, it is common to see the IPS function integrated into firewalls. Just like IDS, there are Network-based IPS (NIPS) and Host-based IPS (HIPS).



	  NIDS	NIPS --> Firewall --> Router --> Internet
		|	|
Server --> Switch --> Wireless Access Port --> Laptops and Tablet
			|
		Workstations and phone