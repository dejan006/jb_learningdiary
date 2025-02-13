# Automate Infrastructure Concepts
----------------------------------------

## Concept 1: VRO
VRO executes / implements workflows such as setting up a server or a VM after it has been requested by a person.

Workflow: 
- Flowchart with start and end and intermediate steps such as approvals, setting up VMs, active directories, etc.
- Shows what needs to be done. 

---> Problem: They put things there, but leave them there without further support

---> To solve this there is a second option: Fleet commander

## Concept 2: Fleet Commander

If a User requests a VM with customized sizes of CPU, etc., he has to do it now in Git and not in form of a Workflow (Clicking on a UI).

---> Advantage: This requested stays there and will not be forgotten after some time (3 weeks for example).

Now the Commander can read this wish request and decomposes it. For example he takes the wish for a VM and decomposes it into multiple Units: Active Directory, Network and VM). The Unit takes the blueprint and knows what they have to do.

The method that Fleet Commander uses is called "**reconciliation**". Reconciliation defines de desired state and tries to get there step-wise, without losing the original state.

### First Difference
- In the first concept, the owner can say "I want it like that" and the team has to do the entire job. 
- With second Method out team does the Commander part and helps with a Unit, but each Owner has to do their own Unit.

### Second Difference
I mentioned that the request is not in the Git and won't be forgotten after some time. This gives the opportunity to change something and it will be automatically changed for everything, because the commander goes through it every few minutes and sees if something needs to be changed. Also if I delete something the commander will see that something is missing and will just replace it with a new one. In the first concept I would have to create a ticket for example and mistakes can happen.