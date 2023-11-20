
- it gives graphic view of the processing logic.
- Edges of decision tree = conditions
- Leaf nodes = actions to perform
### Sample
Library Membership Automation Software (LMS) where it support the following options:
- [[Decision Tree#New Member Option|New member]]
- [[Decision Tree#Renewal Option|Renewal]]
- [[Decision Tree#Cancel Membership Option|Cancel membership]]

#### New Member Option
**Decision** - When "new member" option is selected, software asks details about the members's name, address, phone number etc.
**Action** - If proper info is entered then a membership record for the member is created and a bill is printed for annual membership charge plus the security deposit payable.

#### Renewal Option
**Decision** - If "renewal" is chosen, the LMS asks for member's name and his membership number to check whether its a valid member or not. 
**Action** - If membership is valid then membership expiry date is updated and manual membership bill is printed, otherwise error message is display.

#### Cancel Membership Option
**Decision** - "Cancel membership" option is selected, then software asks for member's name and his membership number.
**Action** - Membership is cancelled, a cheque for balance amount due to the member is printed and finally the membership record is deleted from the database.

![[Pasted image 20231120170934.png]]
> Fig. 6.1: Graphical representation Decision Tree of LMS.

## Decision Table
- represents complex processing logic in tabular or matrix form.
- Upper rows - variables or condition to be evaluatd
- Lower rows - actions to be taken
- Column = *rule*
	- implies if the condition is true, then action is to be executed when true.

![[Pasted image 20231120171120.png]]
>Fig. 6.2: Decision table for LMS
>This part for me is super confusing.
### Example
> This would be optional for now.

