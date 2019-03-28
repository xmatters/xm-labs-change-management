# Change Management
This is a process to manage Change Requests using xMatters to automate delivery and processing of approval stages.
Manual approvals process is also supported.
This has been created as a stand-alone feature driven by xMatters but also allows for integration with a third party management system.


<kbd>
  <img src="https://github.com/xmatters/xMatters-Labs/raw/master/media/disclaimer.png">
</kbd>

# Pre-Requisites
* xMatters account - If you don't have one, [get one](https://www.xmatters.com)!

# Files
* [ChangeManagement.zip](ChangeManagement.zip) - This is the Change Management communication plan.  All functionality is delivered with this one file.

# How it works
A Change Manager initiates the 'Request for Change' form entering pertinent details describing the change.  
Properties are available to enter a Change ticket number, change type (Normal or Emergency), status, summary, description, impact, risk, priority, affected service, CI, category, assigned group, backout plan and three sets of approvers
1. Manager approvers
2. Stakeholder approvers
3. CAB approvers

# Installation
Details of the installation go here.

## xMatters set up
1. Steps to create a new Shared Library or (in|out)bound integration or point them to the xMatters online help to cover specific steps; i.e., import a communication plan (link: http://help.xmatters.com/OnDemand/xmodwelcome/communicationplanbuilder/exportcommplan.htm)
2. Add this code to some place on what page:
   ```
   var items = [];
   items.push( { "stuff": "value"} );
   console.log( 'Do stuff' );
   ```


## Application ABC set up
Any specific steps for setting up the target application? The more precise you can be, the better!

Images are encouraged. Adding them is as easy as:
```
<kbd>
  <img src="media/cat-tax.png" width="200" height="400">
</kbd>
```

<kbd>
  <img src="media/cat-tax.png" width="200" height="400">
</kbd>


# Testing
Be specific. What should happen to make sure this code works? What would a user expect to see?

# Troubleshooting
Optional section for how to troubleshoot. Especially anything in the source application that an xMatters developer might not know about, or specific areas in xMatters to look for details - like the Activity Stream?
