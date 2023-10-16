![[Pasted image 20231015222331.png]]
- Most obvious way to develop software.
- It is <mark style="background: #ADCCFFA6;">elegant and intuivetively obvious</mark>, but <mark style="background: #FFB8EBA6;">isn't practical model</mark> in the sense that it can't be used in actual software development projects
- Can be considered to be *theoretical way of developing software*.
- All other SDLC are derived from classical waterfall model.
## Feasibility Study
Aim to determine whether it would be <mark style="background: #ADCCFFA6;">financially and technically feasible to develop a product. </mark>

- At first, project managers/ team leaders try to have rough understanding required to be done by visiting client side. Study different input data to the system and output data produced. They study what kind of processing to be done and look at various constraints on the behavior.
- After the overall understanding, they examine each solution in terms of kind of resources required, cost of development and development time for each solution.
- Based on analysis the pick best and determine whether the solution is feasible financially and technically. They check he customer's budget and whether they have sufficient technical expertise in the area.

## Requirements analysis and specification
Understand the <mark style="background: #FFB8EBA6;">exact requirements of the customer and document them properly</mark>. Consist of two distinct activities:
- **Requirement gathering and analysis**
	- *Goal of gathering* is to collect all relevant info from the customer w/ regards to product to be developed.
	- *Goal of analysis* activity is to collect all relevant data regarding product to be developed from users and customers through interviews and discussions.
- **Requirement specification**
	- User requirements are systematically organized into a Software Requirements Specification (SRS) document


## Design
Transform requirements specified in the SRS document. Having structure that's suitable for implentation in some programming language (PL). Software architecture is derived from SRS document. There's two distinct approaches: 

### Traditional Design Approach
- It consist of two different activities
	- Structured analysis requirements specification
		- carried out where detailed structure of the problem is examined.
	- Structured Design
		- Result of structured analysis are transformed into software design.

### Object-oriented design approach
- Various objects that occur in the problem domain and solution domain first identified.
- Object structure is further refined to obtain detailed design.
## Coding and unit testing
Sometimes called "implementation phase". It is to translate software design into source code.

- Each component is implemented as program module
- End product of this phase is set of program modules are individually tested.
- Module is unit tested to determine correct working of all individual modules.

## Integration and System Testing
Undertaking once they have been coded and unit tested. Modules are integrated in planned manner. Diff modules in software product almost never integrated in one shot.
- Carried out incrementally over number of steps.
- It is tested in every integrated steps partiallly.
- When all modules have been successfully integrated and tested, system testing is carried out.
- Three different kinds of testing activities:

- **α – testing**: System testing performed by the development team. 
- **β –testing**: System testing performed by a friendly set of customers.
- **Acceptance testing**: System testing performed by the customer himself after the product delivery to determine whether to accept or reject the delivered product.

## Maintenance
Requires more effort than necessary to develop the product itself.
- Relative effort of development of typical software product to its maintenance is 40:60 ratio according to pass studies.
- It revolves into three kinds of activities
	- **Corrective maintenance** - Correcting errors that were not discovered during the product development phase.
	- **perfective maintenance** - Improving the implementation of the system, and enhancing the functionalities of the system according to the customer’s requirements. 
	- **Adaptive maintenance** - Porting the software to work in a new environment. For example, porting may be required to get the software to work on a new computer platform or with a new operating system.

## Shortcomings of The Classical Waterfall Model

- Idealistic -assumes that <mark style="background: #FFB8EBA6;">no development error is ever committed</mark> by engineering during phases.
- In reality, engineers commit large numbers of errors every phase.