# BDD Continued.

Potentially written by end users.

There is still ambiguity in Gherkin / Cucumber

Need to map parts of the test to the code.

BDD is simple enough to write

just make it look consistent in tests.

## Gherkin Basics

- Gherkin tests tend to follow a given &rarr; when &rarr; then
- Recommend, The USER does X, not I does X.
- They look best written in present test.
- Logic wise, forces simple tests to be written. noticeably has AND but not OR

### Syntax

- Feature
- Scenario
- steps
	- Given
	- When
	- Then
	- And
- Background
- Scenario Outline
- Comments

#### Feature

- Acceptance tests live inside `.feature` file
- the contain a feature with the form
	- `Feature: the title you give yo the feature`
- For example `CashMachine.feature`
	- `Feature: Cash machine`

#### Scenario

- Derived from the original user story
	- Can be veey abstract or more detiled lower level
- Within a Feature you may have multiple scnarios where the behavior occurs sequentially

**For example:** 

```Cucumber
Feature: Cash Machine
	Scenario: User validates to cash machine
	Scenario: User Withdraws Money
```

#### Steps

- Given: The preconditions (if any)
- When: The trigger actions that occurs
- Then: What happens

```Cucumber
Feature: Cash Machine

	Scenario: User validates to cash machine
		Given User has a card
			And User has PIN
		When Card is Inserted
			And PIN is entered
		Then Check the PIN is correct with bank
```

#### Things you cannot do

- You cannot go backwards
- Has to be Given When Then


#### Background
- Supplies contexts that is true for all scenarios that will follow
- Removes replication of scenario content

#### A problem...

- Copy and pasting the same statement for all possible scenarios is stupid
- Need smarter way to do this.

A better solution using Scenario Outline

- Removes replication of scenario lines
- The angle brackets here are being used as parameter deliminators
- The pipe / vertical bar is being used to define a data table

```Cucumber

Scenario Outline:
	Given User wants to add <item> to their basket
	...


Example:
	| item   | itemTotalAtStart | number | itemTotal|
	| carrot | 4                | 2      | 6        |
	| ...

```

#### Comments

- Gherkin have to be one line
- Has to be its own line
	- `#This is a comment`
- Comments can be used wherever you feel like the situation needs additional information
- `#These scenarios are part of subsystem X`

## BDD Advantages

- Allows broader audience to formulate / inspect tests
- Acts as a bridge between user stories and code tests
- Provide a lightweight paper trail for process definitions

## BDD Disadvantages

- Requires some training
	- Reading Gherkin requires very little
	- Using a testing framework in practice somewhat more
- Where TDD is quite open in terms for test structuring, BDD has to conform with a relatively restrictive language
- Bear in mine the scope of BDD, it ensures code will work but not that it is good code.

**Exam:**
- Do not need to colour Code
- No need to use a tool like notepad++
- SCREENSHOT OF CODE (NEOVIM INSTALL THING)

Homework Exercise
- A security door that uses a PIN code for entry, which 2 users, each of which has their own PIN

# DevOps

- Silo behavior between buisiniess side and dev side produces weak links
	- waterviall via requirement enginner
	- agile via representative stakeholder

### Problems - Lack of shared responsibility after development

- Produces a disjoint between developers and administrators
- Reduces ability to load test using real world data
- Reduces speed of change, and updating
- Isn't an idea solution for complexity or scalability

### Pace

- In Agile 


## DevOps
- Concatenation of Development and Operations
- Started in 2008
- Used by many multinationals
- Borrows Heavily from standard Agile
	- incremental, co-location of devs, small diverse teams, TDD, backlogs
- Commonly utilises service orientation and cloud technology
	- Service orientation - interaction with functionality via an internet accessible interface
	- Cloud - Why run your own servers.
- Reliant on changes to organisation culture
- Reliant on decent tool support.

Always developers on hand to develop / ensure that users don't even realise about change.

## DevOps Practices

1. Enhanced Stakeholder Participation
2. Automated testing
3. Integrated configuration & change management
4. Continuous Integration & deployment
5. Support 
6. Real time monitoring

Many of these break waterfall, DevOps generally based off Agile.

#### Enhanced Stakeholder Participation

- DevOps involves far deeper communication and cooperation between dev staff and operation staff
- Requires culture change. 

#### Automated Testing

- Uses TDD
- Also borrows from others
	- BDD acceptance tests
	- A/B testing etc. for live systems.

#### Integrated configuration & change management

- Developers no longer consider just configuration or change within their own development, but how it will integrate with those around it
	- In real terms this means more dependencies to take into account
	- This streamlines the joint of operations staff in deciding when they can deploy new releases
- Systems allow staff to manage and share information about configuration

#### Continuous Integration & deployment

- Like Agile development but with better tool support

- Integrate changes quickly and deploy quickly with automated support
- Requires a QA gatekeepers and strong tool support
- Far more responsive development but with some added risk.
	- relies on programmers testing code themselves thoroughly before submitting to the repo
- May involve **DARK LAUNCHING**
	- Deployment of features only to selected end users for testing
		- Used by many organisations from Facebook to Tesla.

#### Support

- Recognition of development teams as tier 3 support for a system
	- Tier 0: self help / FAQ
	- Tier 1: Help desk
	- Tier 2: Technicians
	- Tier 3: Development Staff (pick it up like a ticket)
- communal ownership extended. extends ownership beyond deployment
- provides a useful feedback loop for developers

#### Real Time Monitoring

- Integrate existing organisational monitoring infrastructure into new systems
- Proactive monitoring can resolve issues before they become catastrophes
	- For example making logs available to developers
- Dashboards are all about providing intelligence
- For DevOps this can be explored from both Dev and Ops perspectives


#### DevOps Tools

- Those practices require proper tool support leverage
	- Sometime referred to as tool-chains
- Many industries mistakenly believe DevOps is *just* a set of tools
- Jenkins, travis, teamcity, puppet, **chef**, **docker**, AWS, git, ansible, salt

