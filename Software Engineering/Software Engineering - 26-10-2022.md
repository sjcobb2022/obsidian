# Software Testing

Chapter 8 of course desktop covers this.

- Testing is intended to
	- Check operation is as expected
	- Discover Defects
		- Deviations from the requirements
- Tests tend to use artificial data
	- Though it should at least be realistic
	- There is generally an issue with data
		- Limited interaction with an organisation
			- E.g. Companies don't really want to pass you their accounting details

**Can reveal the presence of errors NOT their absence.**

### Types of Tests
- Verification & Validation testes
	- You expect the system to perform correctly using a given set of test cases that **reflects the systems expected use** 
	- A successful test shows that the system **performs correctly**
- Defect Tests
	- Design to expose defects. Can be deliberately obscure and need not reflect how the system is normally used.
	- A successful test is a test that makes the system perform incorrectly and so exposes a defect in the system

Exam style question:
- Could give a test and tell us what type of test it is. 


## Approaches

#### Static Inspections (Static Verification)
 - May be supplemented by tool-based document and code analysis.
	 - E.g. code analysis

#### Dynamic Testing (Dynamic Verification)
- The system is executed with test data and its operational behaviour is observed.

Approaches are complementary.

**Note**: Unless the development and testing teams interact regularly the developers may start to see the testing team as a threat. If they are isolated then they will be seen as threat; have social activities.


## Static Inspections

- No execution of code
- May be applied to any representation of the system (requirements, design, configuration data, test data, etc.)
- Remember inspections check conformance to a specification not conformance to customer needs. (Can't do verification with static inspection)
- Inspections cannot check some non-functional characteristics such as performance, usability...
	- Hard/impossible to determine just from the code

### Advantages

- Incomplete version of a system can be inspected without additional cost
- An inspection can also consider some non-functional attributes
	- Compliance with standards, portability, maintainability.

Software Engineers need to determine which areas of functionally will benefit most from this extra scrutiny.


## Dynamic Testing

 - **Development Testing**, where the system is tested during development to discover bugs / defects
	 - White box testing: You can see which parts of the code break
 - **Release Testing**, where a separate testing team test a complete version of the system before it is released to users.
	 - black box: cannot see what is broken during testing
 - **User testing**, where users or potential users of a system test the system in their own environment.
	 - also black box


### Development Testing

- **Unit Testing**
	- each individual program units or object classes are testing. Testing the functionality of individual objects or methods
- **Component Testing**
	- Where several individual units are integrated to create composite components. Component testing should focus on testing component interfaces
- **System testing**
	- where some or all of the components in a system are integrated and the system is tested as a whole


Classic reductionism.

#### Unit Testing
- Process of testing the code associated with individual components in isolation
- Mainly a defect testing process
- Units may be:
	- individual functions or methods within an object
	- Object classes with several attributes and methods.
- Complete test coverage of a class involves
	- testing all operates associated with an object
	- Settings and interrogating all objects attributes
	- Exercising the object in all possible states

Example

- Need to define test cases for the operations of WeatherStation
- Also using a state model, identify sequences of state transitions to be tested and the event sequences to cause these transitions
- For example
	- Shutdown --> Running --> Shutdown
	- ...

#### Automated Testing

- Whenever possible, unit testing should be automated, makes retesting easier
	- Test automation frameworks such as JUnit are popular
	- Unit testing frameworks provide generic test classes that you extend to create specific

#### Testing Strategies

- Partition testing, where you identify groups of inputs that have common characteristics and should be processed in the same way.
	- You should choose test from within each of these groups.
- Guideline-based testing, where you can use testing guidelines to choose test cases.
	- These guidelines reflect previous experience of the kinds of errors that programmers often make when developing components.


**Example of testing Guidelines**

- Test software with sequence that only hjave single value
- USe sequesnces of diff sizes in diff tests
- derive tests so that the first middle and last elements of the sequence are accessed
- Test with sequences of zero length
- Choose inputs that force the sustem to generate


#### Component Testing

- A compoennts is bigger than a single class, but not equal to the whole system
- Focius on showing that the component interface behaves accoring to its specification
	- Assume tyouy have some user task to perform, What operations in what classes need to work corerctly and in what order? do they?
	- You can assume that uni tests on the individual objects within the component have been completed.

#### System testing

- Exhausitive system testing is impossibe, instead try to providef comprehensive cvoverage of the system
- System testing checks that all copmponents are compativle, interact correctly and treansfer teh right data at the right rime across thewir intergaces
	- For exdampkle test GUI menu functioanlity 
	- Check outputs for a range of common / uncommon scenarios
- System testing can test test the engagement behaviour of a system

What are the non-functional behaviours of the system?

Emergent behaviour of the system.

You can't measure the performance of the system based on each unit.

#### Debugging
- Process
	- Identify bug
	- Find code
	- Analyse code
	- Prove cause
		- Write a test
	- Gather unit tests
	- Fix code
	- Run test

Expensive fix: probably don't fix

### Release Testing

- Testing of deployable solution
- goal: convince supplying company software is ready for deployment
- Usually a black-box testing process where tests are only derived from the system specification
- A separate team that has not been involved in the system development, should be responsible for release testing.


#### Testing the performance of a system

- Part of release testing may involve testing the emergent properties of a system, such as performance and reliability
- Tests should reflect the profile of the use-case of the system
- Load is steadily increased until the system performance becomes unacceptable
- Stress testing is a form of performance testing where the system is deliberately overloaded to test its failure behaviour


## Case study

