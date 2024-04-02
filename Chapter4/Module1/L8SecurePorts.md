## Secure Ports:

Some network protocols transmit information in clear text, meaning it is not encrypted and should not be used. Clear text information is subject to network sniffing. This tactic uses software to inspect packets of data as they travel across the network and extract text such as usernames and passwords. Network sniffing could also reveal the content of documents and other files if they are sent via insecure protocols. Below shows some of the insecure protocols along with recommended secure alternatives.

  ### 21-FTP:
     It uses File Transfer Protocol.
     It is an insecure port.
     Description: Port 21, File Transfer Protocol (FTP) sends the username and password using plaintext from the client to the server. This could be intercepted by an attacker and later used to retrieve confidential information from the server. The secure alternative, SFTP, on port 22 uses encryption to protect the user credentials and packets of data being transferred.
     Secure Alternative Port: 22 - SFTP
     Protocol: Secure File Transfer Protocol.

  ### 23-Telnet:
     It uses Telnet Protocol.
     It is an insecure port.
     Description: Port 23, telnet, is used by many Linux systems and any other systems as a basic text-based terminal. All information to and from the host on a telnet connection is sent in plaintext and can be intercepted by an attacker. This includes username and password as well as all information that is being presented on the screen, since this interface is all text. Secure Shell (SSH) on port 22 uses encryption to ensure that traffic between the host and terminal is not sent in a plaintext format. 
     Secure Alternative Port: 22 - SSH
     Protocol: Secure Shell

  ### 25 - SMTP:
     It uses Simple Mail Transfer Protocol.
     It is an insecure port.
     Description: Port 25, Simple Mail Transfer Protocol (SMTP) is the default unencrypted port for sending email messages. Since it is unencrypted, data contained within the emails could be discovered by network sniffing. The secure alternative is to use port 587 for SMTP using Transport Layer Security (TLS) which will encrypt the data between the mail client and the mail server. 
     Secure Alternative Port: 587 - SMTP
     Protocol:	SMTP with TLS.

  ### 21-FTP:
     It uses File Transfer Protocol.
     It is an insecure port.
     Description: Port 21, File Transfer Protocol (FTP) sends the username and password using plaintext from the client to the server. This could be intercepted by an attacker and later used to retrieve confidential information from the server. The secure alternative, SFTP, on port 22 uses encryption to protect the user credentials and packets of data being transferred.
     Secure Alternative Port: 22* - SFTP
     Protocol: Secure File Transfer Protocol.

  ### 37 - Time:
     It uses Time Protocol.
     It is an insecure port.
     Description: Port 37, Time Protocol, may be in use by legacy equipment and has mostly been replaced by using port 123 for Network Time Protocol (NTP). NTP on port 123 offers better error-handling capabilities, which reduces the likelihood of unexpected errors. 
     Secure Alternative Port: 123 - NTP
     Protocol: Network Time Protocol.

  ### 53 - DNS:
     It uses Domain Name Service Protocol.
     It is an insecure port.
     Description: Port 53, Domain Name Service (DNS), is still used widely. However, using DNS over TLS (DoT) on port 853 protects DNS information from being modified in transit.
     Secure Alternative Port: 853 - DoT
     Protocol: 	DNS over TLS (DoT).

  ### 80 - HTTP:
     It uses HyperText Transfer Protocol.
     It is an insecure port.
     Description: Port 80, HyperText Transfer Protocol (HTTP) is the basis of nearly all web browser traffic on the internet. Information sent via HTTP is not encrypted and is susceptible to sniffing attacks. HTTPS using TLS encryption is preferred, as it protects the data in transit between the server and the browser. Note that this is often notated as SSL/TLS. Secure Sockets Layer (SSL) has been compromised is no longer considered secure. It is now recommended for web servers and clients to use Transport Layer Security (TLS) 1.3 or higher for the best protection.
     Secure Alternative Port: 443 - HTTPS
     Protocol: 	HyperText Transfer Protocol (SSL/TLS).

  ### 143 - IMAP:
     It uses Internet Message Access Protocol.
     It is an insecure port.
     Description: Port 143, Internet Message Access Protocol (IMAP) is a protocol used for retrieving emails. IMAP traffic on port 143 is not encrypted and susceptible to network sniffing. The secure alternative is to use port 993 for IMAP, which adds SSL/TLS security to encrypt the data between the mail client and the mail server. 
     Secure Alternative Port: 993 - IMAP
     Protocol: 		IMAP for SSL/TLS.
	 
  ### 161/162 - SNMP:
     It uses Simple Network Management Protocol.
     It is an insecure port.
     Description: Ports 161 and 162, Simple Network Management Protocol, are commonly used to send and receive data used for managing infrastructure devices. Because sensitive information is often included in these messages, it is recommended to use SNMP version 2 or 3 (abbreviated SNMPv2 or SNMPv3) to include encryption and additional security features. Unlike many others discussed here, all versions of SNMP use the same ports, so there is not a definitive secure and insecure pairing. Additional context will be needed to determine if information on ports 161 and 162 is secured or not.
     Secure Alternative Port: 161/162 - SNMP
     Protocol: 	SNMPv3.
	 
  ### 445 - SMB:
     It uses Server Message Block.
     It is an insecure port.
     Description: Port 445, Server Message Block (SMB), is used by many versions of Windows for accessing files over the network. Files are transmitted unencrypted, and many vulnerabilities are well-known. Therefore, it is recommended that traffic on port 445 should not be allowed to pass through a firewall at the network perimeter. A more secure alternative is port 2049, Network File System (NFS). Although NFS can use encryption, it is recommended that NFS not be allowed through firewalls either.
     Secure Alternative Port: 2049 - NFS
     Protocol: 	Network File System.
	 
  ### 389 - LDAP:
     It uses Lightweight Directory Access Protocol.
     It is an insecure port.
     Description: Port 389, Lightweight Directory Access Protocol (LDAP), is used to communicate directory information from servers to clients. This can be an address book for email or usernames for logins. The LDAP protocol also allows records in the directory to be updated, introducing additional risk. Since LDAP is not encrypted, it is susceptible to sniffing and manipulation attacks. Lightweight Directory Access Protocol Secure (LDAPS) adds SSL/TLS security to protect the information while it is in transit. 
     Secure Alternative Port: 636 - LDAPS
     Protocol: 	Lightweight Directory Access Protocol Secure.
	 
	 