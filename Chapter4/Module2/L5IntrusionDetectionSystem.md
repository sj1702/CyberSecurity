Intrusion Detection System (IDS)
An intrusion occurs when an attacker is able to bypass or thwart security mechanisms and gain access to an organization’s resources. Intrusion detection is a specific form of monitoring that monitors recorded information and real-time events to detect abnormal activity indicating a potential incident or intrusion. An intrusion detection system (IDS) automates the inspection of logs and real-time system events to detect intrusion attempts and system failures. An IDS is intended as part of a defense-in-depth security plan. It will work with, and complement, other security mechanisms such as firewalls, but it does not replace them. 

IDSs can recognize attacks that come from external connections, such as an attack from the internet, and attacks that spread internally, such as a malicious worm. Once they detect a suspicious event, they respond by sending alerts or raising alarms. A primary goal of an IDS is to provide a means for a timely and accurate response to intrusions. 

Intrusion detection and prevention refer to capabilities that are part of isolating and protecting a more secure or more trusted domain or zone from one that is less trusted or less secure. These are natural functions to expect of a firewall, for example.  

IDS types are commonly classified as host-based and network-based. A host-based IDS (HIDS) monitors a single computer or host. A network-based IDS (NIDS) monitors a network by observing network traffic patterns. 



Host-based Intrusion Detection System (HIDS):

A HIDS monitors activity on a single computer, including process calls and information recorded in system, application, security and host-based firewall logs. It can often examine events in more detail than a NIDS can, and it can pinpoint specific files compromised in an attack. It can also track processes employed by the attacker. A benefit of HIDSs over NIDSs is that HIDSs can detect anomalies on the host system that NIDSs cannot detect. For example, a HIDS can detect infections where an intruder has infiltrated a system and is controlling it remotely. HIDSs are more costly to manage than NIDSs because they require administrative attention on each system, whereas NIDSs usually support centralized administration. A HIDS cannot detect network attacks on other systems.


Network Intrusion Detection System (NIDS):

A NIDS monitors and evaluates network activity to detect attacks or event anomalies. It cannot monitor the content of encrypted traffic but can monitor other packet details. A single NIDS can monitor a large network by using remote sensors to collect data at key network locations that send data to a central management console. These sensors can monitor traffic at routers, firewalls, network switches that support port mirroring, and other types of network taps. A NIDS has very little negative effect on the overall network performance, and when it is deployed on a single-purpose system, it doesn’t adversely affect performance on any other computer. A NIDS is usually able to detect the initiation of an attack or ongoing attacks, but they can’t always provide information about the success of an attack. They won’t know if an attack affected specific systems, user accounts, files or applications.


Security Information and Event Management (SIEM):

Security management involves the use of tools that collect information about the IT environment from many disparate sources to better examine the overall security of the organization and streamline security efforts. These tools are generally known as security information and event management (or S-I-E-M, pronounced “SIM”) solutions. The general idea of a SIEM solution is to gather log data from various sources across the enterprise to better understand potential security concerns and apportion resources accordingly.

SIEM systems can be used along with other components (defense-in-depth) as part of an overall information security program.







Narrator: Here we see an example of an Intrusion Detection System (IDS) alert. This is being provided as an example of how threats are identified, Some of the concepts in this scenario are more advanced than this course, so don’t be alarmed if you don’t understand everything discussed here.

We’ll start by reviewing the main points of the data that is presented to us. Note that in this example, the hostname and username fields have been removed to maintain anonymity.

This tells us that the IDS detected the use of software called Advanced IP Scanner that can be used by attackers to enumerate, or look through the network, scanning addresses to see what services are running on the computers in the local network. This software is also used by network or system administrators to inventory a local network for troubleshooting purposes. Finally, this top section of the alert screen tells us that the event was reported by an endpoint agent, meaning that it was generated by a Host Intrusion Detection System (HIDS) solution, not a Network Intrusion Detection System (NIDS).

This line identifies the host that is running the suspicious process as a Windows system.

This process section identifies the start time, process name and ID (or pid) number that correlates to the process in the Windows Task Manager. This can be helpful in a couple of ways. First, the start time tells us how long the process has been running. The pid can also give some clues, as lower pid numbers may indicate a process that started running during the boot sequence and higher numbers indicate something that was started much later.

These lines give us the details of the executable file, including the path to the file itself as well as the actual command line that was used to run the executable. These are important contextually as they show the program executed from a Temp folder under the user’s ID, which typically does not require administrative privileges in a Windows system. In other words, they could be run by any average user. The command line used shows additional context, including that the application is running as a portable application, meaning that it doesn’t have to be formally installed on the machine to execute.

In this case, there is not enough context to really know if this process is being used in a malicious manner. Like many security alerts, this one relies on some human interaction, so you should contact the end user assigned to this asset to inquire whether they are, in fact, running this software and if they have a legitimate business reason to do so. If you discover that this was intended, it might be a good place to explain to that you were alerted because this legitimate software can be used by threat actors to conduct reconnaissance on the local network to determine where there might be weaknesses to exploit.



