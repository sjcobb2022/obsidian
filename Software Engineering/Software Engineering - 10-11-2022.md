# UML Use Cases

The use case approach complementary to written requirements. Do not replace requirements with this though.

Diagrams are drawn to show
- Which users (called actors) interact with system
- What they want the system to do.

1. Use case describe what functions the system should provide from the perspective of the users.
2. Use case diagrams are often supported by Use Case descriptions; document interaction between users and system. 

Ensure that they are kept up to date; living documents.

Once other diagrams are done some Use Case descriptions are unnecessary.

### Example

**Use cases**

A use case is the need for a actor to interact with the system which, when fulfilled, should yield a result of measurable value.

big arrow from user to cash machine.

"Withdraw cash"
- Use case description


## Notation.

- No arrow head on connecting line
- Actors are outside system boundary.
- Use case names generally active verbs and a noun: "Withdraw (verb) Cash (noun)"

#### Think about actors

- Actors defined as someone or something that is outside the system but that interacts with it.
- **Note:**
	- Actors are not always people
	- Other systems that interact with this system but that are OUTSIDE the system boundaries also called "Actors"
	- External systems are automatically actors.
	- Use cases generally attached to the actors (little not underneath)

#### Think about system boundaries.

Can put as many system boundaries there as possible. 

- need to know how to label it, draw it. etc.

## Specialisation / Generalisation

- Association is just a line.
- E.g. Engineer and Bank Manager are both staff members
- More information (permissions in this case) that is given by the type of user. Engineer has greater access for ex.
- Arrow always goes towards the general form.
- Engineer
	- maintain machine
	- check for damages
- Bank Managers
	- Check for Damage
	- Fill Cash Machine
- The Staff member therefore has a single association line to the check damage which engineer and bank managers then inherit from.

### Use Case Diagrams

- Implications of inheritance of behaviour. 


## Other relationship arrows

Line:
- basic association line

Dotted line:
- Include
- Extend

### \<\<Include \>\> Dependency

- Monitoring security dependent on login to system.
	- "Can't monitor security unless logged into system"
- Raise alarm also dependent on login system.
	- "Can't raise alarm without being logged in"

- Indicates that entire transaction monitoring system will fail unless we implement the staff login system.

### \<\<Extend\>\> Dependency

- Raise Alert "Extends" Monitoring security.
	- dotted arrow from raise alarm to monitoring security.

#### Example
- Manage Bank account
	- points of extend: send payment, check statement
- Send Payment
	- extends manage bank account 
- Check Statement
	- extends manage bank account

### What we don't want

- Overuse of include arrows
- They are used for critical dependencies that are not necessarily obvious (this is unfortunately a grey area)
- Use case diagrams are not designed to show sequences of activity, we have other diagram types for this

Extend vs total subset.
- Extend only adds functionality
- total subset inherits all variables and functions.

## Multiplicities

- Numerical representation
- Instantiation information into a use case diagram

**UML Multiplicity Guide**:
| Numerical Representation | Textual Representation  |
| ------------------------ | ----------------------- |
| 0                        | no instances whatsoever |
| 0..1                     | zero or one instances   |
| 0..\* \| \*              | zero or more instances  |
| 1                        | exactly one instance    |
| 1..\*                    | one or more instances   | 


"How many times a user can interact with the software in a single transaction"

- Customer can manage bank account as many times as they want. (1 -> 1..\*) Have to interact at least once.
- A Bank manager may be involved in transaction (0..1), they can only manage one bank account at any given time (1). 

### Examples

**Cafe Customer**
- 1 customer can make 0..\* order food transactions
- 1 customer can make 0..\* order drink transactions

**Bank Customer**
- 2 customers can open 0..1 joint account


## Use Case Descriptions
- Generally 1 per diagram
- Used at start of a project.

### Example diagram

| Action                | Data                                                                                                                                                        |
| --------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Use Case Name         | using  cash machine                                                                                                                                         |
| Written by            | name, date                                                                                                                                                  |
| Updated by            | name, date                                                                                                                                                  |
| Principle Actor       | customer                                                                                                                                                    |
| Other Actors          | InterBank Network System                                                                                                                                    |
| Trigger               | customer wants to access money                                                                                                                              |
| Description Breakdown | Customer approaches machine, Customer inserts card, Customer gives correct pin on request, Customer decides how much money they want, System checks balance |
| Sequence              | sequential happens in order                                                                                                                                 |
| Outcomes              | customer takes money if they had enough

## Good and bad Use Case naming

**Photographer Bad Example**
- Open Shutter 
- Flash
- Close Shutter

**Photographer Good Example**:
- Take Picture
- Download Picture

Use Cases *must* be  from the Actor’s  (external) Perspective.

### Developing Use Cases

- Use Case identification is an Iterative and Incremental process
- Consider
	- Which functions does the actor require from the system? What does the actor need to do?
	- Does the actor need to read, create, destroy, modify, or store some kind of information in the system?
	- Does the actor have to be notified about events in the system,  or does the actor need to notify the system about something? What do those events represent in terms of functionality?
	- Could the actor’s daily work be simplified or made more  efficient through new functions in the system (typically functions currently not automated in the system)?

