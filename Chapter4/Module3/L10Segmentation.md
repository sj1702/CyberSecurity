Segmentation for Embedded Systems and IoT
An embedded system is a computer implemented as part of a larger system. The embedded system is typically designed around a limited set of specific functions in relation to the larger product of which it is a component. Examples of embedded systems include network-attached printers, smart TVs, HVAC controls, smart appliances, smart thermostats and medical devices. 

Network-enabled devices are any type of portable or nonportable device that has native network capabilities. This generally assumes the network in question is a wireless type of network, typically provided by a mobile telecommunications company. Network-enabled devices include smartphones, mobile phones, tablets, smart TVs or streaming media players (such as a Roku Player, Amazon Fire TV, or Google Android TV/Chromecast), network-attached printers, game systems, and much more. 

The Internet of Things (IoT) is the collection of devices that can communicate over the internet with one another or with a control console in order to affect and monitor the real world. IoT devices might be labeled as smart devices or smart-home equipment. Many of the ideas of industrial environmental control found in office buildings are finding their way into more consumer-available solutions for small offices or personal homes.  

Embedded systems and network-enabled devices that communicate with the internet are considered IoT devices and need special attention to ensure that communication is not used in a malicious manner. Because an embedded system is often in control of a mechanism in the physical world, a security breach could cause harm to people and property. Since many of these devices have multiple access routes, such as ethernet, wireless, Bluetooth, etc., special care should be taken to isolate them from other devices on the network. You can impose logical network segmentation with switches using VLANs, or through other traffic-control means, including MAC addresses, IP addresses, physical ports, protocols, or application filtering, routing, and access control management. Network segmentation can be used to isolate IoT environments. 


Narrator: The characteristics that make embedded systems operate efficiently are also a security risk. Embedded systems are often used to control something physical, such as a valve for water, steam, or even oil. These devices have a limited instruction set and are often hardcoded or permanently written to a memory chip. For ease of operating the mechanical parts, the embedded system is often connected to a corporate network since and may operate using the TCP/IP protocol, yes, the same protocol that runs all over the internet. Therefore, it is feasible for anyone anywhere on the internet to control the opening and closing of a valve when the networks are fully connected. This is the primary reason for segmentation of these systems on a network. If these are segmented properly, a compromised corporate network will not be able to access the physical controls on the embedded systems.  The other side of the embedded systems, which also applies to IoT devices, is the general lack of system updates when a new vulnerability is found. In the case of most embedded systems with the programming directly on the chips, it would require physical replacement of the chip to patch the vulnerability. For many systems, it may not be cost-effective to have someone visit each one to replace a chip, or manually connect to the chip to re-program it.   We buy all these internet connected things because of the convenience. Cameras, light bulbs, speakers, refrigerators, etc. all bring some sort of convenience to our lives, but they also introduce risk. While the reputable mainstream brands will likely provide updates to their devices when a new vulnerability is discovered, many of the smaller companies simply don’t plan to do that as they seek to control the costs of a device. These devices, when connected to a corporate network, can be an easy internet-connected doorway for a cyber criminal to access a corporate network. If these devices are properly segmented, or separated, on the network from corporate servers and other corporate networking, a compromise on an IoT device or a compromised embedded system will not be able to access those corporate data and systems.  




Microsegmentation
The toolsets of current adversaries are polymorphic in nature and allow threats to bypass static security controls. Modern cyberattacks take advantage of traditional security models to move easily between systems within a data center. Microsegmentation aids in protecting against these threats. A fundamental design requirement of microsegmentation is to understand the protection requirements for traffic within a data center and traffic to and from the internet traffic flows. 

When organizations avoid infrastructure-centric design paradigms, they are more likely to become more efficient at service delivery in the data center and become apt at detecting and preventing advanced persistent threats. 


Narrator: Some key points about microsegmentation:  Microsegmentation allows for extremely granular restrictions within the IT environment, to the point where rules can be applied to individual machines and/or users, and these rules can be as detailed and complex as desired. For instance, we can limit which IP addresses can communicate to a given machine, at which time of day, with which credentials, and which services those connections can utilize.   These are logical rules, not physical rules, and do not require additional hardware or manual interaction with the device (that is, the administrator can apply the rules to various machines without having to physically touch each device or the cables connecting it to the networked environment).   This is the ultimate end state of the defense-in-depth philosophy; no single point of access within the IT environment can lead to broader compromise.   This is crucial in shared environments, such as the cloud, where more than one customer’s data and functionality might reside on the same device(s), and where third-party personnel (administrators/technicians who work for the cloud provider, not the customer) might have physical access to the devices.  Microsegmentation allows the organization to limit which business functions/units/offices/departments can communicate with others, in order to enforce the concept of least privilege. For instance, the Human Resources office probably has employee data that no other business unit should have access to, such as employee home address, salary, medical records, etc. Microsegmentation, like VLANs, can make HR its own distinct IT enclave, so that sensitive data is not available to other business entities, thus reducing the risk of exposure.  In modern environments, microsegmentation is available because of virtualization and software-defined networking (SDN) technologies. In the cloud, the tools for applying this strategy are often called “virtual private networks (VPN)” or "security groups.”  Even in your home, microsegmentation can be used to separate computers from smart TVs, air conditioning, and smart appliances which can be connected and can have vulnerabilities.