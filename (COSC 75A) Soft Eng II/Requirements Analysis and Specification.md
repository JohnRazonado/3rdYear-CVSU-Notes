**System Analyst** - experienced member of dev team that understand and document exact requirement of the customer.

- Analyst starts *requirement and analysis* act by collecting all info from the customer.
- Analyzes the collected info to understand, remove all ambiguities and inconsistencies from initial customer perception.
The following basic question can pertains to the analyst grasp of the problem:
- What is the problem? (background of the study)
- Why is it important to solve the problem? (SOP)
- What are the possible solutions to the problem? (Objectives)
- What exactly are the data input to the system and what exactly are the data output by the system? (Context flow diagram [Diagram that gave birds eye view])
- What are likely complexities that might arise while solving the problem? (Somewhat part of methodology)
	- If there are external software or hardware with which the developed software has to interface, then what exactly would the data interchange formats with the external systems be? (Hardware interaction to system).

- After analyst understood the exact customer requirements, it then proceeds to identify and resolve various problems. Most important part has to identify, and eliminate problems of anomalies, inconsistencies, and incompleteness. 
## Parts of [[Modeling|SRS]] Document
- Functional requirements of the system
- Non-functional requirements of the system
- Goals of Implementation

### Functional Requirements
 - functionalities required from the system
 - System is considered to perform high-level functions $\left\{ f_{i} \right\}$.
 - Having the transformation of sets of input data $\left\{ i_{i} \right\}$ that corresponds to set of output data $\left\{ o_{i} \right\}$

![[Pasted image 20231120142230.png]]
> Fig. 5.1: View of system performing set of functions
### Nonfunctional Requirements
- deal w/ **characteristics of the system** that can't expressed as functions.
- Sample
	- Security
	- Efficiency
	- Portability
	- ISO requirements

### Goals of Implementation
- Documents general suggestion of regarding development.
- Guide for trade-off among design goals
- Document issues such as revisions, new device to support, reusability, etc.
### Identifying Functional Requirements from a Problem Description
- high-level functional requirements needed to be identified by either from **informal problem description document** or **conceptual understanding** of the problem.

#### Sample
Consider the case of library system

**F1**: Search Book Function
**Input**: An author's name
**Output**: Details of author's book and location of book in the library.

So the function *Search Book* (F1) takes the author's name and transforms it into book details.
## Documenting Functional Requirements
- Need to specify the set of functionality suported by the system.
- Function can be identified states
	- data input to the system
	- input data domain
	- output data domain
	- type of processing


## Properties of Good SRS Document
- **Concise** - at the same time unambiguous, consistent, and complete
- **Structured** - well-structured in general. Document is easy to understand and modify. Since SRS documents undergoes several revisions
- **Block-box view** - Specify what the system should do and refrain stating to do these. It should specify only the external behavior of the system.
- **Conceptual Integrity** - Having reader to easily understand it
- **Response to undesired events** - Acceptable responses to undesired events. Called *"system response to exceptional conditions"*.

## Problems W/out SRS Document
- Not be implemented according to customer needs
- Software devs wouldn't know if they're developing what's exactly required by the customer
- Difficult for the maintenance engineers to understand functionality of the system
- Difficult for user document writer to write user's manual

## Problems w/ An Unstructured Specification
- Very much difficult to understand document
- Very much difficult to modify document
- Conceptual integrity isn't shown
- SRS document might unambiguous and inconsistent.


