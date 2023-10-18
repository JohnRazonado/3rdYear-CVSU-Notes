>Part of Configuration Management Standards to Quality Factors of QC (Page 10 to 33)

- CM should always based on standards applied **w/in an organization**.
- Should define how:
	- items **identified**
	- changes **controlled**
	- versions **managed**
- Should be based on **evolutionary process** model rather than like a **waterfall model**.

### Standards (approved by ANSI)
- **IEEE 828**: [[Configuration Management|Software Configuration Management]] Plans
- **IEEE 1042:** Guide to Software Configuration Management




## Consideration of Configuration
| | | Platforms|
|---|---|---|
|Baseline (Title)|Desktop App|Main Frame Version (Unix, Windows Server)|
|^^| ^^|Work Station Version|
|^^|Mobile App|Windows Version| 
|^^|^^|Android Version|
|^^|^^|IOS Version|
|^^|Web App|Client/Server|

![[Pasted image 20231010213930.png]]

IT = Information Systems
CS = Software Product

#### Conflicts
- **Simultaneous updates** - how to prevent one person undoing changes of another
- **Shared and common code** - how to notify everyone needing to know the change
- **Versions** - how to make changes to all affected.

## Software Configuration Items
1. **Computer Program**
	- both source and executable
2. **Documentation**
	- Both technical and user
3. **Data**
	- w/in a program or external to it

### Examples of Configuration Items
- Product concept specification
- Software project plans
- Software requirements specifications
- Software design descriptions
- Source code
- Database descriptions
- Software release processes
- Software test documents
- User documentation
- Maintenance documentation
- etc.

## Software Configuration Management Tasks
- **Identification**
	- **Tracking of multiple version** enabling efficient changes
- **Version Control**
	- **Control changes** before and after release of customer
- **Change Control**
	- Authority to approve and **prioritize changes**
	- Intended to the [[Review (1-3)#^50fbfa|Change Control Board]]
- **Configuration Auditing**
	- Ensure change made properly.
- **Reporting**
	- Tell other about changes made.



### Version Control
- Combines procedures and tools managing different **versions of configuration objects** created.

#### Variant
- Different set of object at same revision level.
- Can co-exist w/ other variant.
#### Version
- Separated from one another
- new versions defined when **major changes** happened to **one or more objects**.

## Version and Release Management
#### Invent identification scheme for system versions
 - version **numbering**
 - attribute-based **identification**
 - **change**-oriented identification
#### Plan new release is to be produced
- Needed to plan on a gantt chart
#### Ensure that version management procedures and tools are applied properly
- Identify items that could be culprit of a bug (prediction)

## Configuration Management Activities
### Configuration Item Identification
- modeling of the system as a set of **evolving components**.
#### Promotion Management
- Creation of version for other **developers**
- Integration of tech by other company.
#### Release Management
- creation of versions for **clients and users**
#### Change Management
- Handling,approval, and tracking of **change request**
#### Branch Management
- Management of **concurrent development**
#### Variant Management
- management of version **intended to coexist**

#inProgress 
> Need to update and summarize stuffs here.
### Configuration Planning
- List of **scheduled baseline** version releases
- List of [[Configuration Management Standards#Software Configuration Items|SCIs]] (documents, code, etc.) to be included in each version
- Table identifying relationship of software development project and maintenance plans to scheduled **releases of new SCI or SCI versions**.
- List of assumptions about **resource required to perform [[Configuration Management Standards#Software Configuration Management Tasks|SCMP]]**.
- **Estimates** of **human resources and budget** needed to perform SCMP.
<br>
- Defines *types of documents* to be managed and document naming scheme.
- Defines *who takes responsibility* for CM procedures and baseline creation.
- Defines *policies for change* control and version management
- Describes *tools* which should used to assist CM process.
#### Configuration Management Roles
#### Configuration Manager
- Defining procedures for creating promotions and releases
#### Change Control Board Member
- Approving or rejecting change request
#### Developer
- Creates promotion triggered by request
#### Auditor
- Selection and evaluation of promotions for releases.
- Ensuring consistency and completeness.
- Like QC/QA

### Change Management
- handing of **change request**
	- Change request leads to creation of new releases.
- Complexity of change management process varies the project.
- Small projects can perform change request informally and fast
- Complex projects require detailed change request form and official approval by one or more managers.
- Two types of controlling change:
	- **Promotion:** **Internal development state** of a software is changed (by developers).
	- **Release:** Changed software system is **made visible outside** the development organization(by users)
- General change process
	- **Change is requested** (can be done by anyone including users and developers)
	- Change request is **assessed against project goals**
	- Following the assessment, **change is accepted or rejected**
	- If its accepted, change is assigned to **developer and implemented**
	- Implemented **change is audited**

#### General Change process
> Need the detail info

1. **Change Request**
	- Specifies procedures for requesting change to baselined CI and info to be documented:
		- Name(s) and version(s) of the CI(s) where problem appears
		- Originator's name and address
		- Date or request
		- Indication of urgency
		- The need for change
		- Description of requested change
2. **Evaluation of Change**
	- Specifies analysis required to determine **impact of proposed change** and procedure reviewing the results
3. **Change approval or disapproval**
	- This section of SCMP describes organization of ***configuration control board (CCB)***
		- Can be individual or group
		- Multiple levels of CCBs are possible, depends on the complexity of the project.
		- Multiple levels of CCBs may be specified
			- In small development efforts one CCB level is sufficient
	- Also indicates level of authority of CCB and its responsibility
		- SCMP must specify when CCB is invoked
4. **Implementing Change**
	- Section of SCMP where specifies activies for verifying and implementing approved change
	- Completed change request must contain the ff info:
		- Original change request(s)
		- Names and versions of the affected configuration items
		- Verification date and responsible party
		- Identifier of new version
		- Release and installation data and responsible party
	- Must also specify activities for:
		- Archiving completed change requests
		- Planning and control of releases
		- How to coordinate multiple changes
		- How to add new CIs to the configuration
		- How to deliver new baseline.

### Quality Factor
- Configuration Management (CM) ensures current design and build state of the system is known, good & trusted.
- It enhance quality may also refer as quality factors are given below:

1. **Increase Efficiency**
	- stability, and control by improving visibility and tracking
2. **Cost Reduction**
	- Detailed knowledge of all elements of configuration
	- Allows unnecessary duplication to be avoided.
3. **Enhanced system reliability**
	- Rapid detection and correction of improper config could negatively impact performance
4. **Ability to monitor and audit**
	- define and enforce formal policies and procedures govern assets identification, status **monitoring, and auditing**
5. **Greater agility**
	- faster problem resolution
6. **Decreased risk**
	- greater levels of security
7. **Faster restoration** of service.