
# Exam structure

part A: UML (20 marks)
- problem solving
- 2-3 diagram types

part B: everything else (40 marks)
- mix

2  mins per mark

Define patters and anti-patterns providing examples for each(4 marks)
definition
example
definition
example

Discuss implications of patter/anti-pattern identification and use (2 marks)
implication 1
implication 2

USE BULLET POINTS

Upload sample answers after revision week. 

# The London Ambulance Disaster

LASCAD

systems are complex and small issues in design implementation, planning had issues.

600 s1aure miles 318 miles

2000 calls per day

just wasted 7.5m in automated system.
- 300% over budget

Existing system:
- calls taken by operators
- details written down on card
- slotted onto high speed conveyer belt to radio operators
- radio operators communicate with ambulance
- Time waiting for operator to answer phone: 5 seconds, processing time around 3 minutes
	- new gov requirements wanted 3 minutes turnover time

**The vision**
- Data links to ambulances
	- digital screens
- Early mapping software to automate routing of nearest ambulance
- reduce staffing, de-skill staff significantly
- cost a minimum of 1.5m
- would take min of 19 months
- need hardware + software + control center
- 35 bids

**Tendering process**
- anything over 1.5m is bad!
	- this left 1 bidder which was a consortium
	- System Options was left with 35k for software dev
	- never developed real time system or safety critical systems before
	- staffordshire ambulance service said not to use 
- they make the project lead System Options
- 700,000 pounds lower than the nearest bidder
- offered bespoke system (from scratch)
- Cut development time in half

**Approach**
- Design was complete after 6 months for impl and testing
- used PRINCE for the first time (actually just said they were doing it)
- they had no QA for their change management process, just did stuff without telling LAS



**The technology**
- Ambulance links could handle voice or data (but not both simultaneously)
- choice of programming languages
	- use VisualBasic launch edition
	- microsoft literally said not to do it
- use monolithic development approach

**Stakeholders interactions**
- 2 managers who managers the bidding process who had no IT experiences
	- one knew he was about to be made redundant
	- other was temporary contractor
- all requirements written by 2 managers
- acceptance testing is a good idea?
	- outsourced acceptance testing to development company

**What happened**
- Systems are quite complex to develop
	- Fell behind schedule so they gave up with testing
	- gave up with system testing
	- Hope that they would work togehter
	- no load/stress testing at all
	- Decided all of a sudden to 3 phase development

Unplanned Phasing
- Phase 1/2: supported call handling and dispatch
	- removed the conveyer belt...
	- had to hire literal runners
- Phase 3: Electronics, automated dispatch etc.
	- launched at 5 am
	- sluggish...
	- on launch there were 81 known bugs
	- routing software blind to one way streets
	- no way for operators to override the systems choice of ambulance 
	- there was no way of knowing if an ambulance had already been routed.
	- Sends 11 ambulance to one street because it was shit software...

**Unknown bugs?**
Equivalence partitioning is important
- Every 53rd ambulance was invisible.
- Multiple calls led to multiple ambulances
- Messages were routed to ambulance screens but no scroll function was implemented
	- only way to get the info back was to radio which lost track of location
- More ambulances use radio to counteract data problems, lost ambulance positioning
- Visual Basic 1.0 had very bad memory leak
	- killed system completely
	- 20 min wait time
	- 11 hours for ambulance response time

**The aftermath**
- Deaths?
	- no one knows
	- estimated 30-40

- Funeral director beat an ambulance to an incident

- LAS did eventually computerise
	- in 2006 computer crash sent staff temporarily back to paper and pens.

- Bad software development issue.

 