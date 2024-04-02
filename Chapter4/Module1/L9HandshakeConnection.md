Narrator: Between the client and the server, there is a system for synchronizing and acknowledging any request that is known as a three-way handshake. This handshake is used to establish a TCP connection between two devices.   Here, we will take a simplified look at how communications are established to a web server. Depending on the exact protocol, there may be additional connection negotiation taking place.   First, the client sends synchronization (SYN) packet to the web server’s port 80 or 443. This is a request to establish a connection.  The web server replies to the SYN packet with an acknowledgement known as a SYN/ACK.  Finally, the client acknowledges the connection with an  acknowledgement (ACK). At this point, the basic connection is established, and the client and host will further negotiate secure communications over that connection. 
	 

Matching Ports with Their Secure Counterparts: 

Which of the following protocols is a secure alternative to using telnet? (D4, L4.1.2) 
 A. HTTPS
Incorrect. HyperText Transfer Protocol Secure is the secure alternative for HTTP and uses SSL/TLS for securing website communications.

 B. LDAPS
Incorrect. Lightweight Directory Access Protocol Secure (LDAPS) is the secure alternative for Lightweight Directory Access Protocol (LDAP) and is used to exchange directory information in a secured protocol.

 C. SFTP
Incorrect. Secure File Transfer Protocol (SFTP) is the secure alternative to FTP and is used to transfer files.

 D. SSH
Correct. Secure Shell (SSH) is the secure alternative to telnet as it encrypts all traffic between the host and remote user.