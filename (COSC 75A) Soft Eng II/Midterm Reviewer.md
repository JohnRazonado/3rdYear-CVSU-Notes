> This is the reviewer released by the professor.

## Configuration Management
**Three main types of software releases**
- **Baseline version**
- **Intermediate version**
- **Revisions**

Baseline Version – are the biggest and planned early.
Intermediate Version – designed to address the immediate problems as to correct defects.
Revisions – minor changes and corrections

  
**Software Configuration items**
- Computer Programs
- Documentation
- Data

**Software Configuration management task**
**Identification**
**Version Control**
**Change Control**
**Configuration auditing**
**Reporting**

  
**Variant** – Different set of objects at the same revision level.

  
## Software Engineering

**Software** is considered to be a collection of executable programming code, associated libraries and documentations.

**Software product –** software made for a specific requirement.

**Engineering -** about developing products, using well-defined, scientific principles and methods.

**Software engineering** as an engineering branch associated with the development of software product using well-defined scientific principles, methods and procedures.

**CHARACTERESTICS** **OF** **GOOD** **SOFTWARE**
- Operational
- Transitional
- Maintainable

### Operational
This tells us how well software works in operations. It can be measured on:

- Budget
- Usability
- Efficiency
- Correctness
- Functionality
- Dependability
- Security
- Safety
### Transitional
This aspect is important when the software is moved from one platform to another:
- Portability
- Interoperability
- Reusability
- Adaptability
### Maintenance
This aspect briefs about how well a software has the capabilities to maintain itself in the ever- changing environment:

- Modularity
- Maintainability
- Flexibility
- Scalability 

## SDLC

Software life cycle model (also called process model) is a descriptive and diagrammatic representation of the software life cycle.

## **Different** **software** **life** **cycle** **models**
1. Classical Waterfall Model
2. Iterative Waterfall Model
3. Prototyping Model
4. Evolutionary Model
5. Spiral Model

Classical waterfall model is intuitively the most obvious way to develop software.
![[Pasted image 20231121010343.png]]
**Feasibility study** - The main aim of feasibility study is to determine whether it would be financially and technically feasible to develop the product.

**Requirements analysis and specification: -** The aim of the requirements analysis and specification phase is to understand the exact requirements of the customer and to document them properly.

**Design: -** The goal of the design phase is to transform the requirements specified in the SRS document into a structure that is suitable for implementation in some programming language.

**Coding and unit testing:-**The purpose of the coding phase (sometimes called the implementation phase) of software development is to translate the software design into source code.

**Integration and system testing: -**Integration of different modules is undertaken once they have been coded and unit tested.

**Maintenance: -** Maintenance of a typical software product requires much more than the effort necessary to develop the product itself.


**ITERATIVE** **WATERFALL** **MODEL** - To overcome the major shortcomings of the classical waterfall model, we come up with the iterative waterfall model.
![[Pasted image 20231121010403.png]]
  
  

A **prototype** is a toy implementation of the system.

_PROTOTYPING MODEL_
![[Pasted image 20231121010445.png]]

**EVOLUTIONARY MODEL** - It is also called _successive versions model_ or _incremental model_.
![[Pasted image 20231121010500.png]]
  
  

**SPIRAL MODEL** - diagrammatic representation of this model appears like a spiral with many loops.
![[Pasted image 20231121010516.png]]
##### First quadrant (Objective Setting)
- During the first quadrant, it is needed to identify the objectives of the phase.
- Examine the risks associated with these objectives.

##### Second Quadrant (Risk Assessment and Reduction)
- A detailed analysis is carried out for each identified project risk.
- Steps are taken to reduce the risks. For example, if there is a risk that the requirements are inappropriate, a prototype system may be developed.
##### Third Quadrant (Development and Validation)
- Develop and validate the next level of the product after resolving the identified risks.
##### Fourth Quadrant (Review and Planning)
- Review the results achieved so far with the customer and plan the next iteration around the spiral.
- Progressively more complete version of the software gets built with each iteration around the spiral.

## Requirement Analysis and Specification
**_System analysts_** - Experienced members of the development team carry out this job.

The analyst starts _requirements gathering and analysis_ activity by collecting all information from the customer which could be used to develop the requirements of the system.

The following basic questions pertaining to the project should be clearly understood by the analyst in order to obtain a good grasp of the problem:
- What is the problem?
- Why is it important to solve the problem?
- What are the possible solutions to the problem?
- What exactly are the data input to the system and what exactly are the data output by the system?
- What are the likely complexities that might arise while solving the problem?
- If there are external software or hardware with which the developed software has to interface, then what exactly would the data interchange formats with the external system be?


The important parts of SRS document
1. Functional requirements of the system
2. Non-functional requirements of the system,
3. Goals of implementation

**Functional requirements** part discusses the functionalities required from the system.

**Nonfunctional requirements** - deal with the characteristics of the system which cannot be expressed as functions - such as the maintainability of the system, portability of the system, usability of the system, etc.

**Goals of implementation** part documents some general suggestions regarding development.