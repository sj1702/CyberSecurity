Redundancy
The concept of redundancy is to design systems with duplicate components so that if a failure were to occur, there would be a backup. This can apply to the data center as well. Risk assessments pertaining to the data center should identify when multiple separate utility service entrances are necessary for redundant communication channels and/or mechanisms.  

If the organization requires full redundancy, devices should have two power supplies connected to diverse power sources. Those power sources would be backed up by batteries and generators. In a high-availability environment, even generators would be redundant and fed by different fuel types. 

									|------ UtilityPower
  |----------|-----TransferSwitches-|
UPS1		UPS2					|---Generator--Motor--Fuel
  |			 |
UPS3		UPS4					|------ UtilityPower
  |----------|-----TransferSwitches-|
									|---Generator--Motor--Fuel
									
									
									
Narrator: In addition to keeping redundant backups of information, you also have a redundant source of power, to provide backup power so you have an uninterrupted power supply, or UPS. Transfer switches or transformers may also be involved. And in case the power is interrupted by weather or blackouts, a backup generator is essential. Often there will be two generators connected by two different transfer switches. These generators might be powered by diesel or gasoline or another fuel such as propane, or even by solar panels. A hospital or essential government agency might contract with more than one power company and be on two different grids in case one goes out. This is what we mean by redundancy. 


