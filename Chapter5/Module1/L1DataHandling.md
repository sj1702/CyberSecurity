Data Handling:
Data itself goes through its own life cycle as users create, use, share and modify it. Many different models of the life of a data item can be found, but they all have some basic operational steps in common. The data security life cycle model is useful because it can align easily with the different roles that people and organizations perform during the evolution of data from creation to destruction (or disposal). It also helps put the different data states of in use, at rest and in motion, into context. Let’s take a closer look. 

All ideas, data, information or knowledge can be thought of as going through six major sets of activities throughout its lifetime. Conceptually, these involve: 
	- Create:
	Creating the knowledge, which is usually tacit knowledge at this point.
	
	Store:
	Storing or recording it in some fashion (which makes it explicit).
	
	Use:
	Using the knowledge, which may cause the information to be modified, supplemented or partially deleted.
	
	Share:
	Sharing the data with other users, whether as a copy or by moving the data from one location to another.
	
	Archive:
	Archiving the data when it is temporarily not needed.
	
	Destroy:
	Destroying the data when it is no longer needed.
	
	



Narrator: Data handling is extremely important. As soon as we receive the assets, the data we need to protect, we need to make sure we know the best practices for handling this data.   First, we need to recognize which assets we need to protect. This is based on the value of the data according to the owner of that data. Based on that, we see what kind of risk we are facing with respect to the likelihood that this information could be compromised, destroyed or changed by any means, and what vulnerabilities exist that we need to account for. This is the life cycle of data handling, from create, to store, to use, to share, to archive and finally to destroy. And at any point there are different risks to the data and different practices for handling it. Some of these procedures are mandated by government standards.  For example, in the US, the Occupational Safety and Health Administration (OSHA) is the federal government agency that protects the well-being of workers. Under the rules of the Healthcare Insurance Portability and Accountability Act (HIPAA), medical records need to be kept for 10 years, but under OSHA, if we have a medical record of an on-the-job injury, that record needs to be maintained for over 30 years, even after the last day of work in that particular organization. That’s a regulatory requirement, and if you don’t know that or don’t abide by it, you can find yourself in trouble as the result of an audit. So you can see that we have to be very cautious when deciding how to handle data, as there may be multiple regulations that apply to a single piece of data.   Also in the US there are also specific guidelines related to the Payment Card Industry Data Security Standards (PCI DSS) requirements regarding credit card information and how to maintain that information securely. In the European Union, the GDPR also has specific requirements regarding the handling of financial data. In order to protect the data properly, you need to know all the relevant requirements for the type of data being protected in the various geographic areas.  Many countries and other jurisdictions have regulations that require certain data protections throughout every stage of the data’s life cycle. These govern how the data is acquired, processed, stored, and ultimately destroyed. And when looking at the life cycle of the data, we need to keep a watchful eye and protect the information at every stage, even if it’s ready to be legally destroyed at the end of the life cycle. In some cases, multiple jurisdictions may impose rules affecting the data we are charged with protecting. In these instances, we need to be aware of any and all regulations that affect us.  Some data handling practices include classification and labeling, where you determine the sensitivity of the data, what is available to everyone and what needs to be restricted, and label the information accordingly so that your access controls will allow the correct level of access. Retention is how long we store the information and where, based on the requirements of our organization and perhaps regulatory agencies as well. And then there needs to be defensible destruction, meaning that we have the regulatory mandate backing up our decision to destroy the data. Destruction can be physical, of hard drives or computer chips, or destruction of digital records, which can be done under a number of methodologies. We need to make sure we understand the secure destruction of the data, because often we think we can just empty the virtual trash can to delete the data. But when we do that, old emails and other data may never be erased. To completely erase the data on physical media, you need to use some technical equipment for degaussing, such as powerful magnets to erase the data stored on tape and disk media such as computer and laptop hard drives, diskettes, reels, cassettes and cartridge tapes. However, an individual with sophisticated equipment could potentially still retrieve that information, at least partially. So we must make sure we understand what recovery tools are available, because if you are subject to regulatory compliance, you have to follow through with specific protocols and processes to destroy that information as required so that it can no longer be accessed in any way.  


Data Handling Practices
Data itself has value and must be handled appropriately.  In this section, we will explore the basics of classifying and labeling data to ensure it is treated and controlled in a manner consistent with the sensitivity of the data. In addition, we will complete the data life cycle by documenting retention requirements and ensuring data that is no longer in use is destroyed. 
	- Classification:
	Businesses recognize that information has value and others might steal their advantage if the information is not kept confidential, so they classify it. These classifications dictate rules and restrictions about how that information can be used, stored or shared with others. All of this is done to keep the temporary value and importance of that information from leaking away. Classification of data, which asks the question “Is it secret?” determines the labeling, handling and use of all data. 

	Before any labels can be attached to sets of data that indicate its sensitivity or handling requirements, the potential impact or loss to the organization needs to be assessed. This is our first definition: Classification is the process of recognizing the organizational impacts if the information suffers any security compromises related to its characteristics of confidentiality, integrity and availability. Information is then labeled and handled accordingly. 

	Classifications are derived from laws, regulations, contract-specified standards or other business expectations. One classification might indicate “minor, may disrupt some processes” while a more extreme one might be “grave, could lead to loss of life or threaten ongoing existence of the organization.” These descriptions should reflect the ways in which the organization has chosen (or been mandated) to characterize and manage risks.  

	The immediate benefit of classification is that it can lead to more efficient design and implementation of security processes, if we can treat the protection needs for all similarly classified information with the same controls strategy. 
	
	
	
	- Labeling:
	Security labels are part of implementing controls to protect classified information. It is reasonable to want a simple way of assigning a level of sensitivity to a data asset, such that the higher the level, the greater the presumed harm to the organization, and thus the greater security protection the data asset requires. This spectrum of needs is useful, but it should not be taken to mean that clear and precise boundaries exist between the use of “low sensitivity” and “moderate sensitivity” labeling, for example. 

	Data Sensitivity Levels and Labels 
	Unless otherwise mandated, organizations are free to create classification systems that best meet their own needs. In professional practice, it is typically best if the organization has enough classifications to distinguish between sets of assets with differing sensitivity/value, but not so many classifications that the distinction between them is confusing to individuals. Typically, two or three classifications are manageable, and more than four tend to be difficult. 

	-Highly restricted: Compromise of data with this sensitivity label could possibly put the organization’s future existence at risk. Compromise could lead to substantial loss of life, injury or property damage, and the litigation and claims that would follow.
	-Moderately restricted: Compromise of data with this sensitivity label could lead to loss of temporary competitive advantage, loss of revenue or disruption of planned investments or activities.
	-Low sensitivity (sometimes called “internal use only”): Compromise of data with this sensitivity label could cause minor disruptions, delays or impacts.
	-Unrestricted public data: As this data is already published, no harm can come from further dissemination or disclosure.



	
	- Retention:
	Information and data should be kept only for as long as it is beneficial, no more and no less. For various types of data, certain industry standards, laws and regulations define retention periods. When such external requirements are not set, it is an organization’s responsibility to define and implement its own data retention policy. Data retention policies are applicable both for hard copies and for electronic data, and no data should be kept beyond its required or useful life. Security professionals should ensure that data destruction is being performed when an asset has reached its retention limit. For the security professional to succeed in this assignment, an accurate inventory must be maintained, including the asset location, retention period requirement, and destruction requirements. Organizations should conduct a periodic review of retained records in order to reduce the volume of information stored and to ensure that only necessary information is preserved. 

	Records retention policies indicate how long an organization is required to maintain information and assets. Policies should guarantee that: 

	-Personnel understand the various retention requirements for data of different types throughout the organization. 
	-The organization appropriately documents the retention requirements for each type of information.
	-The systems, processes and individuals of the organization retain information in accordance with the required schedule but no longer. 
	
	A common mistake in records retention is applying the longest retention period to all types of information in an organization. This not only wastes storage but also increases risk of data exposure and adds unnecessary “noise” when searching or processing information in search of relevant records. It may also be in violation of externally mandated requirements such as legislation, regulations or contracts (which may result in fines or other judgments). Records and information no longer mandated to be retained should be destroyed in accordance with the policies of the enterprise and any appropriate legal requirements that may need to be considered.



	
	-Destruction:
	Data that might be left on media after deleting is known as remanence and may be a significant security concern. Steps must be taken to reduce the risk that data remanence could compromise sensitive information to an acceptable level. This can be done by one of several means:  

	-Clearing the device or system, which usually involves writing multiple patterns of random values throughout all storage media (such as main memory, registers and fixed disks). This is sometimes called “overwriting” or “zeroizing” the system, although writing zeros has the risk that a missed block or storage extent may still contain recoverable, sensitive information after the process is completed.
	-Purging the device or system, which eliminates (or greatly reduces) the chance that residual physical effects from the writing of the original data values may still be recovered, even after the system is cleared. Some magnetic disk storage technologies, for example, can still have residual “ghosts” of data on their surfaces even after being overwritten multiple times. Magnetic media, for example, can often be altered sufficiently to meet security requirements; in more stringent cases, degaussing may not be sufficient. 
	-Physical destruction of the device or system is the ultimate remedy to data remanence. Magnetic or optical disks and some flash drive technologies may require being mechanically shredded, chopped or broken up, etched in acid or burned; their remains may be buried in protected landfills, in some cases.
	
	In many routine operational environments, security considerations may accept that clearing a system is sufficient. But when systems elements are to be removed and replaced, either as part of maintenance upgrades or for disposal, purging or destruction may be required to protect sensitive information from being compromised by an attacker.  


