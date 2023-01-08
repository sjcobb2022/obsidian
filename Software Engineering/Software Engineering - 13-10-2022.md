# Requirements Engineering cont.

ID and descirption about as far as most companies get.

### Rationale 

- Why is this requiremnt important
- Who are you trying to convince?
	- yourself, manager, other RE's, customer
- Without this, a requirement might be modified or even removed without anyone realsing its true reason for existing.

Only a few sentances

in terms of knowledge management
 - otherwise dependant on what is in people's heads.

### Fitness Criteria

- Project success depends on fulfilling the requirements
	- Features that aren't represented by requirements are a sign of creep, bloat, gold plating etc.
- Requirements are only useful if theyt can be checked
	- Did tou provide function X (easy)
	- Does it have a small footprint? (How do you tell)
- The fit criterion states how you go abuot this.


Test first development (vs test driven?)

What makes a sensible test for reliability?

what are non-functional requirement.

If you don't know what test to create then it's proballby a bad test in the first place

#### Importance of Verifiability
- Determining whether a requirement is verifiable what test you would perform...
- Major issues
	- Stakeholders express themselves using: nice, fast, sort of silvery colour
		- not specific data
	- Design tests but don't over constrain
		- e.g. splashproof != waterproof to 5 meters

**Tell you what they want and not what they need.**

Get down to needs rather than wants.

Need to be careful when translating from word to testable number



#### Fit Criteria Examples

**The system must be easy to use.**
- A lousy requirement by itself
	- how do you prove it
- Fit criterion quantifies qualitative statement
- After 10 minutes of training at least 3 of a team of 5 colunteers will be ableto pass an interactice tests of the basic fuctions of a system


**- System will support multiple file formats**
	- Fit criteria: the system will be tested against pdf, jpeg, and docx during testing period
**- programmed in java**
	- check all code in java during testing period
**- System must be secure**
	- the complainst with security standards ABC
**- respond to queries in 5 seconds**
	- respond to queries over first few months of operations, check for compliance with response times.

### Owner
- Despite out effots requiremtns are not entirely self contained
- Assigneing an owner confers responsibulityu
	- someone knows why a requirement is there  and whther it could be modified or even removed
- E.g. Elon Musk is a big believe in personal responsibility in Research Engineering. 
	- easier to assign blame.

### Classifying requirements

- User level
	- readoable by everyone
	- do not use complex technical terms, not condescending
	- There should be high level coverage of the whole system at a user level
- System leve
	- Readable subject to technical expertise
- Some classifiers have rules attached there a requirement cannot be both system and user level

large grey area in who understands what. E.g. the user may understand system level and vice versa it depends.

**User level**
- 4.5 the shystem will not provide door access control
- 4.8 the system must allow administrative access for management

**System level**
- 6.2 system will use a dedicated control system
- 6.3 The sustem will provide command line interface for administration.
	- 6.3.1 Each door will have it's own ACL
		- careful with acronyms




#### Functional or non-functioanl requiremtns

Functional
 - Statements of services the sustem should provide
 - "Here is the code that does that"

Non-functional is it
- How fast is it, how long is the testing period, what language was used, what tools used

**They are mutually exclusive**. A requirement cannot be both functional and non-functional (if you think it is probably conflation).
- Normally 2 requirements stuck together, which should be seperate

**Example for non-functional: CATIA 4 vs CATIA 5 for wiring of Boeing A380**

##### Functional requiremnts
Functionaluser requiremnts may be hihg-level statements of waht sustem should do
- LEARN will provide a file upload facility

Functional system requirements should be used to describe the system services in detail
- LEARN should do a virus scan on files


##### Functioanl requiremnts: an underspecified system

- The doors shall have a data link to the fire control system
- The alarn should sound if unauthorised movement is detected
- The door system will maintain an audit log
	- the audit log will contain Ids, logged times, and entry / exit points

Burglar alarm kept on going off.

Don't let them in again if they didn't swipe out.

No one could get back into the building.

System was a complete catastroophe



#### Non-Functional Requirements

Known as the '-ilities'

- Cover broad areas
	- system properties
		- Reliability, response time, storage requiremnts. I/O device capability
	- Requirements may also be specifinc mandating a particular method (but only where absolutely necessary)

- Non functioanl requiremnts may be more critical than functioanl requireements
	- Door example failed non-functional: too slow

8.2 A door should exhibity a failure on demand of less that 10*



### Requiremtn keywords: FURPS+
- Most popular industry method
	- Functionality
		- Feature set, Capabilities, Security
	- Usability
		- Human factors, Aesthetics, Consistency,  Documentation
	- Reliability
		- Frequency/severity of failure, Recoverability,  Predictability, Accuracy, Mean time to failure
	- Performance
		- Speed, Efficiency, Resource consumption,  Throughput, Response time
	- Supportability
		- Testability, Extensibility, Adaptability,  Maintainability, Compatibility, Configurability, Serviceability,  Installation, Portability
- Any given requirements may apply one or more of these tags.


### Volatility

- Enduring requiremnts
	- stable requiremtns derived from the core actiicvet of the customers organisation
- Volatile requiremnts
	- Requiremnts which change during development or when the sustem is in use
	- Managin volatile requiremnts is tricky.
- Mutually exclusinve, cannot be both enduring and volatile, would indicate conflation.

### Importance: MoSCoW

- M
	- must describe a requirement that must be satisfied
	- Minimal Usable SubseT
- S
	- should: represents a hugh-priority requirement
- C
	- could: describe a desirable but non-essential requirement
- W
	- Won't
		- we avoid the expanding horizon issue by using these only for downgraded, must, should could.



- A unique identifier  
- A requirement description  
- A requirement rationale (why are you doing it?)  
- A level (User / System)  
- Requirement keywords (FURPS+)  
- Fit Criteria 
- Volatility 
- Priority  
- Owner  
- A few others for good measure  
	- History, Dependencies, Associated documents

## Example

Unique ID: #23  
- Description: The system MUST include a mySQL database  
- Rationale: Databases are the most efficient method of storage,  and the Empire already use mySQL  
- Classification: System, Functional, Enduring, Functionality,  Performance  
- Fit Criteria: Calls will be made to the database during testing.  
- Owner: Roger the Rabbit  
- History: Introduced 1/11/2009 by Roger the Rabbit, Modified  3/4/2010 by Kermit the Frog Priority: MUST  
- Dependencies: Req #56, Req #88

- Unique ID: #44  
- Description: The Deathstar WON’T have a cupholder  
- Rationale: Cupholders would be useful, but are not necessary  to crush the rebel alliance  
- Classification: User, Functional, Volatile, Usability  Fit Criteria: The cupholder would be tested using common cup  sizes  
- Owner: Darth Vader  
- History: Introduced 1/11/2256 by Darth Vader, Modified  3/4/2256 by Emperor Palpatine  
- Priority: Low, not planned in this version  (low-medium-high not MoSCoW)
- Dependencies: Req #54, Req #67



Structured formats can make identifying data easier.

### Case study

**NASA**

Mars Polar Landaer
- Launched 1999
- $110 Million 
- Designed to land in the polar region
- Splattered after 470M miles of travel

**The descent** 

- Three landing legs each with magnetic touchdown sensors which are periodically checked.
- If the sensors indicate touchdown for two consecutuve readings then the inidication is considered valid
	- Indicated set to True
	- Descent engine shutdown
- System testers discovered that klanding leg deployment (at altitude 1500m) caused suprios touchdown signals 
- Created a system requiremnt that said that the use of sesor data should not begin till 40m from the surface
- Sensor readings still sampled will before 50m to keep processor demands constant

- New system requirements wasnt properly translated into a software requirement
- System requirement
	- Explained what the system should do diff
	- Did not explain why
- Hence software developers
	- Adaped thesofware not to use sensor data before 40m
	- Did not know there would be incorrect sensor data.
	- At exactly 40,m engine turned fof because boolean was switched.