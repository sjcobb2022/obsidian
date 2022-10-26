Reuiqwmrenets confuction
- Functuional and non0-functional requirements rend to get mixed-up
	- east ro use is not a functio dagnabiut
	- and its not a good non functional either
- Requierment confgaltion 
	- seceeral requiremnts may be expressed togethwer and need seperatin g out
		- The door system must provbide acces to all members or the departmern dat and night, through the use of specifci coded keyfobs and entry cards. It will also allow administarros to manage the system
		- TOO MUCH INFO

Requirement imprecision

 - Requirements arise when problems not speificially stated
- Ambihguous requriemnents may be interpreted in different watys by developers and users

**Shoot the officer on no account shoot the dog.**

Imprecision can be dur tyo mistaken expectaitons
- Users think the internet and the web are the same
- users are unaware of anything other than Windows exists

## Term Overloading

Actronym SME?
- Small Medium Size Enterprises
- Subject Matter Expert
- Special Materials Expert
- Social Market Economy
- The iSO stander for the klanguge covering lapland
- Glossaries are rather important....


## Requirement interaction

 - Conflicts between different non-functional requiremnts are common in complex systems
 - Spacecraft
	 - To minimise weight, the number of sepearete chips in the sustem should bne minimised
	 - To minimise power consumptions, lower power chips should be used
	 - However using lower power chips may mean that more chips have to be used
	 - Which is teh most ciritical?

## Document and Requirement Management Process

REquirement documetns
- Requirement document is the ofgficial statement of what is required
- Should include both def of user requirements and specification of the system requiremtns
- It is NOT a design document  As far as possible it shoukd se out WHAT the system shoukd do not HOW.

IEEE requirement standard
- Defines generaic structure for requirement docs.
	- Intrio
	- General descruption (UML?)
	- Spcific requriemnts (User and Syste,m)
	- Appendices
	- Index
	- Glossary etc.


### Requirement Managemenr using a Quality Gateway 
- Key feature of Volere
- Decide if requirements makes the cut
	- Accept
	- Reject
	- Ask for clarification
- Based on speciifc criteria: completemenes, value, traceability, testability, consistency, viability
- Learning process
- suppoes to be quick and not laborious
- Remember requirement and design stages account for abuot 50% of effort.

### Requirement management using requirement reviews

- A quality gateway ensures the quality of an individual requirements
- How do you ensure the voerall speicifcation is on track? Preiodic requirement reviews
	- Helkp find problenms and aid prioritisation
- Requriements shouldnever be comopletely deelted and form and importatnt input to reviews 
- Regular revuiews should be help while the requirements definition is being formulated 
- Both client and contractor staff shoukld be involved in reviews
- Check verifiability, comprehensability, traceability, adapatability etc.

Fagan reviews are popular

### Tools to support Requirements engineering

- Requirements storage
	- Requirements storage should be managesd in a secure,m manage data store
- Change management
	- The process of change managemebt is a workfow process whose stages can be defgined and information flow between these stages partially atomated 
- Traceability managemebt
	- Automated retrieval of the links between requirements


**There are many different tools!!!** 

Most of them cost money, most of them web based

## Summary

- Requirements Engineering is a key SE activity
- There are specific stages to RE
- Requirements need both specification and categorisation
- There are a number of approaches to RE




# Design Implementation and Approaches


## Phased Replacement

- The old syhstem being a hjelloy, you remove the jelly mould and the organisation is still the same shape. 
- Someone has to change the new users how to use the software.
- the old system embedded in the org 
- training manuals, procurement etc.
- moulding of the org needs to occur.

New software might speeding things up but thats probably not the end of it.



## Benefits of Software reuse

| Benefits                | Explanation                                                                                                                      |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| Accelerated development | reusing software can speed up system production because both development and validation time may be reduced                      |
| Increased dependability | Reused software which has been tried and tested in working systems should be more dependable than new software                   |
| Lower development costs | Development costs are proportional to the size of the software being developed                                                   |
| Reduced process risk    | the cost of exustuing software is already known, therefoire the margin of error in-project cost estimations is rediced           |
| Standards compliance    | Standardisation ensures systems behave ina  similar manner, for example user interface standards, which can reduse user mistakes | 

## Problems with reuse

| problem                                                 | Explanation                                                                                                                                                                                                          |
| ------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Creating maintaining and using a component library      | population and management of component library has significant costs                                                                                                                                                 |
| Finding, understanding and adapting reusable components | software components have to be discovered in a library, understood and sometimes, adapted to work in a new environment                                                                                               |
| Increased maintenance costs                             | If the source code of a reused software system or component is not available then maintenance costs may be higher because the reused elements of the system may become increasingly incompatible with system changes |
| Not-invented-here syndrome                              | Some software engineers prefer to rewrite components because they believe they can improve on them                                                                                                                                                                                                                     |

### Reuse encompasses more than just code

- Documentation may contain
	- Requirements (legal for example), Designs
	- Glossaries
	- Naming conventions and defs
- The main problem here is that SE standards have improved over the years
	- But future  re-use will be easy in comparison.

