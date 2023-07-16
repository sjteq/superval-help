# Sub AddEdit



## HTTP Broker Name

Enter a nickname to be given to the HTTP Request Broker.

## HTTP IP Address

Select the IP Address for the HTTP configuration setup. 

"My Machine" can be selected by all Users but only creates
a "local" Broker on the User's machine which can only be 
accessed by that User. Valuations are carried out on the 
User's machine (in separate instance(s) of SuperVal created 
by the Broker).

"Local IP Address" can be selected by all Users, and if the
User has Administrator rights, other Users who have access
to the IP address can use this Broker for their valuation 
tasks. Valuations are carried out on the User's machine 
(in separate instance(s) of SuperVal created by the Broker).

## HTTP Port

Enter the number for the port for communication.

## HTTP Response Time Limit

Enter the maximum time (in seconds) allowed for the Broker to respond.  

Communications to the Broker will generally be repeated if the response
time limit is exceeded.

## Maximum Number of Sub-Processes

Enter the number of maximum sub processes you want SuperVal to use 
for the Broker.

## HTTP Worker Folder

Select the IP Address for the HTTP configuration setup.

## Worker Memory Allocation

Enter the size of the worker workspace allowance (in MB).

## Abandon "inactive" Workers not heard from for

Specify the number of minutes the "Worker" should wait before abandoning the task
(before becoming inactive).

## Check for "inactive" Workers every

Specify the number of seconds before checking for inactive Workers
(Workers sitting ideally waiting for a task).

## Shut Down idle Workers after

Specify the time (in minutes) before any idle Workers are shutdown.

## OK

When you have finished entering the relevant information, click the _OK_
button to move to the next screen.

SuperVal will check that all of the required entries on the page have
been made. If additional fields require data SuperVal will show briefly
in red which is the first of these fields found on the page.

## Cancel

Clicking on the _Cancel_ button allows you to return to the previous
screen without saving any of your changes.