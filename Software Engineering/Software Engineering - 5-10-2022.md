# SE Cont...

## Globalisation

Geographic spread
- Through collaboration like Airbus or through outsourcing
- Indtorducing new stakeholders

Documentation will most likely be in Englins
- But physica;l meetings may be difficult
- Location, culture, time zone etc all affect the process

Doing so can leverage specialism and lowers costs.

### Thinking Time Zones

Careful preparation allows continual sotware development, IT help etc
- By what if you need synchronoush communication?

### Remote project management

Specialist tools to support user interaction, inlcuding Wikis

### Outsourcing
 **Theory:**
- Expensive in-house
- If you are bad at something,. outsource

**Practice:**
- It can save significant m,oney
- complicates management
- If you were bad at it you can outsource it, but do u have to understand what you have oursourced.


Outsourcing different stages causes different problems

Be careful with quality control issues

#### Case Study: Airbus A380

16 countries involved in development

Involved 4 teams based in 4 different companies

Signicficant delay caused by specification of design tools during wiring design
- Actually a versioning issue.
- Half the aircraft designed with different wiring design.

Minor issue with requirement specification caused major issues.

Rewire 530km of wire. 

#### Case Study: Advanced Passanger Train

Make train tilt whilst making sure no one gets motion fixed.

Software engineers at fault

Designed during summer, implemented in winter.

A lot of people violently ill.

Issue was not taking into consideration the environmet in which the software would be operating.

**Environmental Issue**

#### Case Study:  Patriot Missile System

The use-case was not a good one. 

Kept it running for weeks or days without a restart.

Fired 42 missiles. Reported 41 hits, acutally 0 hits.

Under the impression system was on for a limited time.

Clock-drift problem which caused major issues.

**Insufficient Specification** 


### Summary

Software development is context specific. 



## Software Processes

Software Process Modesl 
- Watervall, V-Model
- Iterative development
- Incremental development
- Re-use
- Software Evolution
- Prototyping

Background reading
- Chapter 2 of course textbook

### Software process

Structured set of activities

- Specification 
- Design / impl
- Validation
- Evolution

A software model is an abstract representation of a process.

### Plan-driven vs Agile processes

Most practical process include both elements of plan and agile approahches

Based on context and environment


### Plan Driven Software

Waterfall model
 - Plan driven model, seperateand disticnt phases of specification and development
VModel
- waterfall with added emphasis on testing
Iterative development
- may be plan-driven or agile
Incremental development 
- may be plan driven or agile
Intergration and configuration
- The system is assembled from existing configurable components. May be plan-driven or agile.


#### Waterfall model

Requirements analysis and definition  
- System and software design  
- Implementation and unit testing  
- Integration and system testing  
- Operation and maintenance

Build it in chunks


#### V-Model

Split design into a bunch of finer individual, signed-off, chunks.

Sofware engineers write the tests a lot earlier on. 

Helps ensure legitemacy of testing.

Broken the system down so much that going back down is a lot more complicated.

#### Incremental Development

Dewvelop system sin parts, each part providing some useful function to the customer

Could be imagined as multiple mini waterfalls if plan driven.

**Advantages**
- Reduce costs of change
- Debugging easier
- Easier to get feedback
- Rapid delivery and deployment possible
- Customers are able to use and gain vale from the software earlier than is possible with a waterfall process.

**Disadvantages**
- Increased cost of change for past increments
- Inevitability more complex for management
- costs will be higher


#### Iterative develoment

Works from a higher level desing
 - build parts of the system iteratively
 - could include developing some parts multiple times to improve them
 - Can be used within phases of riggid systems such as waterfall (but not across)

Advantages
- Good for prototyping risky or badly understood functionality
- Potential for ongoing geedback

Disadvantages 
- More flexible than the waterfall model, but still rigid between iterations
- Expensive if sustem was well understood
- not cost effecive
- system structure can degrade.