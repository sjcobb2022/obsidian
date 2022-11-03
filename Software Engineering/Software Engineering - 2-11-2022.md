# Agile Software Development cont.

XP has weakness of centralised control.

## Background to Refactoring

Convectional wisdom: design for change. Spend time and effort anticipating changes before you start to reduce costs later in the life cycle.

XP Wisdom: conventional wisdom is wasteful and very slow.
- Instead proposes less planning, more action, utilising continual code improvements.

### Refactoring

Programming team look for possible software
- improves the understandability of the software and reducing the need for documentation
- Changes are easier to make because the code is well-structured and clear
- Remove unnecessary complexity

Some changes require architecture refactoring


## Pair Programming

- Pair programming involves programmers working in pairs, developing code together
	- pars are dynamic during development
- Helps develop common ownership of code and spreads knowledge
- Pro vices an informal review process (each line of code is looked at by more efficient than 1 person)
- Pair programming is more efficient that 2 programmers working separately.

## Agile customer involvement in TDD

- The customer helps write the acceptance tests for the stories that are to be implemented in the next release
- Customers have limited time
	- Have to be dedicated to make it work.
- Customers always engaged!
	- (but they have limited time)

Stress was common in early agile development.


small releases : XP got this right, 2 weeks 

Pair programming: XP got this wrong, works in theory but not popular.

Continuous intergration: as soon as a task is complete, it is integrated into the whole system.

Sustainable pace: XP got this wrong, 2 weeks way too short

On-site customer: XP got this very wrong. contactable yes, on-site is a bit too much



# Agile Development Techniques: SCRUM

A lot more flexible than XP.

Phases
- Initial
	- Outline planning phase (objectives and software structuring)
- Sprints
	- Where each sprint develops an increment of a system, Each sprint should be a shippable piece of functionality.
- Closure
	- Documentation (manuals etc.) + lessons learned.

Reuses similar concepts to XP
- **User Stories**
- **Refactoring**
- **Small Teams**
- **Collective Ownership**
- **TDD**



## Teamwork in Scrum

- The **Scrum Master**
	- a facilitator who arranges daily meetings, tracks the work to be done, records decisions, measures progress and communicates with customers and management outside of the team.
- A **backlog** is maintained containing the set of user stories still to be implemented
	- user stories have 'effort points' attached allowing the **velocity** of a given sprint to be determined
	- Effort points are not time periods as such, they are relative only to each other in a backlog.
		- probably should be time based
	- if not in the current increment, they are in the backlog
- Daily short progress meetings are held (scrums)
	- Everyone therefore knows what's going on
	- make sure that the scrums don't take too much time
	- 5-10 mins at the beginning of the day.

## The sprint cycle

- Sprints are fixed length, generally longer than XP
- The starting point for planning is the backlog, which is the list of work to be done
- The developers and customers then decide what is going to be develop in that increment.


## Scrum benefits

- The product is broken into manageable chunks
- Unstable requirements do not hold up progress
- The whole team have visibility of everything
- Customers see benefits whit every increment 
- Promotes mutual trust


## Scrum Drawbacks

- training and on-boarding is sensitive
	- team changes can effect moral, hard to integrate.
- scrum master is a tricky job
- daily meetings can take up valuable resources, restricting team size
- not all projects suit an incremental development cycle conducive with Scrum
- close ties depend on team co-location
	- teleconferencing is a poor substitute.


## Case Study

Sometimes agile is used where it isn't necessarily applicable.

UK Universal Credit

Make agile instead of plan-based (the firm was plan-based)

Turned out the company wasn't very good at revolutionising their work systems.

12 years of lifecycle.

## Summary

- "I'll go and fine out what they need and the rest of you start coding"



# Behaviour Driven Development

Mainly used in a test-driven environment.

Get the end users to run tests?

Abstracting a test to the point at which the end-user can write the tests.

Very cutdown version of BDD.

Can be implemented by different software tools.

- BDD technical collaboration between technical and non-technical teams
- BDD addresses two big problems:
	- Agile User stories are simple, informal, and convey a good amount of Requirement Engineering related information
		- ID,
	- Agile emphasises customer involvement through development.
		- py-test or something isn't very


- Written in Natural English Language descriptions
- Focuses on providing suitable unit and acceptance tests which are executable.
- BDD came from TDD
- TDD uses code, BDD uses structured language
- Like TDD it requires good tool support.

## BDD Basics

- BDD does not specific format
- languages have emerged (Gherkin)
- Agile User Stories are often starting points for BDDs

## Three Phases
1. Discovery
	- Explore Behaviour Through discussions between owner/developer
	- through workshops
	- **Output: Verbally Agreed Behaviour**
1. Formulation
	- Create a test in natural language.
	- **Output: Acceptance Test**
1. Automation
	- Coded in BDD. 
	- **Output: Executable Acceptance Test**

- Note: Like mane SE artefacts, BDD tests are living documents, if you change some thing you should update them!

