## Open Source developmet as a form of reuse

An appreach to sopfware developmmnt on which the source code of a sogware system is published and colunteers are invited to paririciparte in the development process

Its roots are in the free sofware foundation
- Adovates that source code should not be proprietary

Open source sofweare really took off with the Internet, allowing the recruitment and coordination of a much larger propulation of volunteer developers.


GNU-OS?? 


The best known open source sustem is Linux
Other important open source projects
 - Wordpress
 - Java
 - Apache web server
 - mySQL 
 - OpenOffice
 - Blender

### Open source business

More and more prioduct comaprnies are uising an open source approach to development
- their business ,models are not reliant on selling a sopfrware product but selling uspport for tha product
- They believe tha tinvolving ht eopen source communirt will allow softerware to be developme more quickli cheaply...

Open source licensing.
 - A fundamental principle of open source is the source should be freely available
	 - Legally the developer of the code still owns the code. They can place restrictions of how it is ues
	 - Some open oource developesrs bnelieve that if an open osuirce compoenets is used to develop should all be free


#### Common License Models

- GNU GPL (General Public Licensse). Called reciprical license which means that if you use open source sofweare that is licesnsed under the GL liccesnse then tyoyu ust make htat sotware open source.
	- Contagious disease of open source.
- The GNU Lesser General Public Licesns (LGPL) os a cariante of the GPL where you cam write components that link to open source code wothout having to publish 
- Berekely Standard Distribution (BSD) License. non-reciprocal license. Which means you are not ibliges to republish any changes opr modifications made to open source. youcan include the code in proprietary sustems that are sold.


### Enterprise Software 

COTS Software is used for many things.

### ERP systems
- Enterpricereousrce planning
	- Can cover many buisioess areas
		- Everyhting can marketing to delviver routes
	- ERP is a subset of COTS in business functionality
		- Frequently seen to encompass supply chain management
	- Biggest ERP companies?
	- Has existed for teh past 25 or so in manufacturing 45 years ago or so.
- Harness shared databases for efficiency.

#### Configurtation and Customisation

 - We know configuration is cheaper than customisation
 - So why might we perform customisation?

#### Implications of ERP

- Using prebuildt models
	- Invetibale compormises
	- Idenrtiftyin closts fit
	- Novelty vs Cost
	- In theory reduce sots & increase speed
	- Embodies best practice?
- Changes role of SE but does not eliminate it.

Significant proportion of ERP deployment is failure. Not the sopftware but the way that it is used / deployed.

#### Case study

 - Classical case study
	 - FoxMeyer (Pharmaceuticals)
		 - Worth 5 billion
		 - management expected a silver bullet, automation, affected employee morale, unrealistic deadlines, costs, resources etc.
		- Use SAP for new system (warehouse distribution system)
		- Use 3rd Party for consulting
		- Wanted to revolutionise the business in 18 months
		- Charged 100 million dollars for the system.
		- In deployments the system misplaced $34million in shipments.
			- never found
		- Skipped the entire system testing.
		- FoxMeyer sued SAP for $500 million
		- needed 420k transactions per day. could only do abuot 10k
		- By the time SAP were sued, FoxMeyer ceased to exists.
		- Went form $5billion to $80 million
- 40% partial failure, 20% outright failkure for 


### CRM systems
- Customer Relationship Management
- Focuses on customer interaftions and sales
	- Mannages contacts, leads
	- Provide workflow for communications
- Biggest players?
	- Salesforce (30% of market). Adobe, Oracle, SAP


## The rise of low code no code platforms

- Point and click rpgram
- 14 billion a year on the market
- alreadty has CMS for website consuction. VB.net for drag and drop user interfaces?
- Hundreds of platforms available including Bubbles, Appian, Betty Blocks

produce quite poor-quality code 


#### Will LCNC take over?

 - Depends on def of take over
 - CMS decimated the role of rpogrammers in small web dev
	 - for LCNC it is inevitbale they will take over small, quick 


## Architectural Patterns 

"Use your previous knowledge"

- Exploit commonality
- Well understood characteristics
	- Known for efficienct or resiliance for example
- Pattersn can be positive or negative
- Pattern experts are highly prized on projects.

pattern = good way to architect a system
anti-pattern = bad way 

##### Examples
- Model View controller
- Client server architectuire
- Event driven a
- polling
- plugin 
- service oriented
- transaction based
- peer-to-peer
- etc.etc.

**Example:** MVC
- For GUI designs
 - Allows for multiple presentations of an object and separate interactions with these presentations.

**Example:** Client server
- have a client, ahve a server, they talk over a network

#### Anti-Patterns

- Big ball of mud, not recongnisablew
- Gold plating - adding unnecessary features
- Stovepipes - system which cannot talk to each toher
- God objects - centralising everything.
- Mushroom management
	- programmers keypy in the dark up to their necks in shit

### Patterns, the good, the bad and the ugly...

- Constrianing
- Emergence over time 
- Common re-use
	- peer to peer architectures will most likely contain leements relating to decentralisation
	- sevice oriented architectures will contain elements relateing to web interfaces.
- 

#### Code Smells
- Where anti=-pattersn cover poor architectiure, code smells are more techincal implementation issues
	- Dead code
	- innefficnet
	- poor excessive commenting
	- Poor method naming
	- replicated code
	- very long methods
	- code that that is difficult ro mainta
- A smell is not a bug but it still isn't a good sign.


## System Reliability

- Everything has a scale attached

### Common measurements for system reliability

- MTTF - Mean time to Failure
- MRRT - Mean time to Recovery
- MTBF - Mean time between failures
- MTBF = MTTF + MTTR
- Availability = MTTF / (MTTF + MTTR)
- Implications: Impact on designed, Severity, Timing, Independance of components.


Ab=vailability is ofern in the form $10^2$

e.g. means 0.99 availability (3.56 days a year)

Issues
- The public don't understand it
- Someone has to come up with the facts to support it
- Complex system failure is very rarely binary.

Changing risk perception means means that systems should be better...

**The 70's saw two reliability approaches emerge**

Triple Modular Redundancy
 - Designed for unrealiable hardware
 - had 3 seperate versions and then had a vote.

N version programming. 
- Have multiple versions and then vote on the changes.


### Why is Speed so often an issue

- In order to get someone to develop a system to a cost tou need to be abl to specifit the load on that sustem
- But load may vary by
	- Time of dat
	- Time of year
	- External factors such as failures / disasters
	- Success of the company
- Suystemare therefore dwesignd for peak load
- If you modify processing adding funcrtions to grow the business ot can be difficult to calculate.

