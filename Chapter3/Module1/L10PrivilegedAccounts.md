Privileged Accounts
Privileged accounts are those with permissions beyond those of normal users, such as managers and administrators. 

Broadly speaking, these accounts have elevated privileges and are used by many different classes of users, including: 

Systems administrators, who have the principal responsibilities for operating systems, applications deployment and performance management. 
Help desk or IT support staff, who often need to view or manipulate endpoints, servers and applications platforms by using privileged or restricted operations. 
Security analysts, who may require rapid access to the entire IT infrastructure, systems, endpoints and data environment of the organization. 
Other classes of privileged user accounts may be created on a per-client or per-project basis, to allow a member of that project or client service team to have greater control over data and applications. 

These few examples indicate that organizations often need to delegate the capability to manage and protect information assets to various managerial, supervisory, support or leadership people, with differing levels of authority and responsibility. This delegation, of course, should be contingent upon trustworthiness, since misuse or abuse of these privileges could lead to harm for the organization and its stakeholders. 

Typical measures used for moderating the potential for elevated risks from misuse or abuse of privileged accounts include the following: 

More extensive and detailed logging than regular user accounts. The record of privileged actions is vitally important, as both a deterrent (for privileged account holders that might be tempted to engage in untoward activity) and an administrative control (the logs can be audited and reviewed to detect and respond to malicious activity). 
More stringent access control than regular user accounts. As we will see emphasized in this course, even nonprivileged users should be required to use MFA methods to gain access to organizational systems and networks. Privileged users—or more accurately, highly trusted users with access to privileged accounts—should be required to go through additional or more rigorous authentication prior to those privileges. Just-in-time identity should also be considered as a way to restrict the use of these privileges to specific tasks and the times in which the user is executing them. 
Deeper trust verification than regular user accounts. Privileged account holders should be subject to more detailed background checks, stricter nondisclosure agreements and acceptable use policies, and be willing to be subject to financial investigation. Periodic or event-triggered updates to these background checks may also be in order, depending on the nature of the organization’s activities and the risks it faces. 
More auditing than regular user accounts. Privileged account activity should be monitored and audited at a greater rate and extent than regular usage. 


Explore Further:
Let's consider the Help Desk role. In order to provide the level of service customers demand, it may be necessary for your Help Desk personnel to reset passwords and unlock user accounts.  In a Windows environment, this typically requires “domain admin” privileges.  However, these two permissions can be granted alone, giving the Help Desk personnel a way to reset passwords without giving them access to everything in the Windows domain, such as adding new users or changing a user’s information. These two actions should be logged and audited on a regular basis to ensure that any password resets were requested by the end user. This can be done by automatically generating a daily list of password resets to be compared to Help Desk tickets. This scenario allows the Help Desk personnel to resolve password-related issues on the first call while doing so in a safe and secure manner. 