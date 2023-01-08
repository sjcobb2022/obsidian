# Object Diagram

Real world data in a application of class.

- Don't have multiplicity or type beyond association.
- A transfer of class diagrams into simpler form.

Sherlock's Account : Customer is the naming scheme

# Sequence Diagrams

Use cases: understand how people interact with the data

Focus purely on message flow. Nothing about what the system is doing.

Semantically similar but visually different.

## Interaction type Diagrams

Interaction diagrams outline the messages and data passed between objects and actors.

Time down dot arrow

Box for objects.

Actor as stickman

Slides have elements.

Instantaneosus communication and non instantations messages

Instantaneous : straight to the right/left, angled otherwise.

Angled through time. 

## Synchronouse and Asynchronouse MEssages

- Sequence diagams allow the developer to specify the behaviour of the system on sending/receiving messages.
- Synchronous: wait for next message to process at receiveing end before moving to next step.
- Asynchronos: Don't wait, get on with next step: more responsive but requires thought.

Examples: 
- Verbal: Sync
- Email: Async
- Phone: Sync
- Post: Async
- Social Media Chat: Async 


## Creating things

| Good                               | Bad |
| ---------------------------------- | --- |
| records, transactions, receipts... | databases, people, websites, systems, buildings.    |

## Destroying Things

| Good                              | Bad |
| --------------------------------- | --- |
| Temporary: sessions, transactions, instances | Static: people, websites, systems...    |



