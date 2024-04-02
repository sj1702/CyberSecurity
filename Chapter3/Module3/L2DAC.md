Discretionary Access Control (DAC)
Discretionary access control (DAC) is a specific type of access control policy that is enforced over all subjects and objects in an information system. In DAC, the policy specifies that a subject who has been granted access to information can do one or more of the following:

Pass the information to other subjects or objects 
Grant its privileges to other subjects 
Change security attributes on subjects, objects, information systems or system components 
Choose the security attributes to be associated with newly created or revised objects; and/or 
Change the rules governing access control; mandatory access controls restrict this capability 

Most information systems in the world are DAC systems. In a DAC system, a user who has access to a file is usually able to share that file with or pass it to someone else. This grants the user almost the same level of access as the original owner of the file. Rule-based access control systems are usually a form of DAC. 

DAC Example:
Discretionary access control systems allow users to establish or change these permissions on files they create or otherwise have ownership of.

Steve and Aidan, for example, are two users (subjects) in a UNIX environment operating with DAC in place. Typically, systems will create and maintain a table that maps subjects to objects, as shown in the image. At each intersection is the set of permissions that a given subject has for a specific object. Many operating systems, such as Windows and the whole Unix family tree (including Linux) and iOS, use this type of data structure to make fast, accurate decisions about authorizing or denying an access request. Note that this data can be viewed as either rows or columns:
 -An object’s access control list shows the total set of subjects who have any permissions at all for that specific object.
 -A subject’s capabilities list shows each object in the system that said subject has any permissions for.
		
		AccessControlList for ExcelFile1
		
			^
			|
		
		ExcelFile1			ExcelFile2
 Aiden	Read/Write/execute	Read/execute	--> Aiden's Capabilities List
 Steve	Read				Read/Write


This methodology relies on the discretion of the owner of the access control object to determine the access control subject’s specific rights. Hence, security of the object is literally up to the discretion of the object owner. DACs are not very scalable; they rely on the access control decisions made by each individual object owner, and it can be difficult to find the source of access control issues when problems occur.


DAC in the Workplace:
Most information systems are DAC systems. In a DAC system, a user who has access to a file is able to share that file with or pass it to someone else. It is at the discretion of the asset owner whether to grant or revoke access for a user. For access to computer files, this can be shared file or password protections. For example, if you create a file in an online file sharing platform you can restrict who sees it. That is up to your discretion. Or it may be something low-tech and temporary, such as a visitor’s badge provided at the discretion of the worker at the security desk.


