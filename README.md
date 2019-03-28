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

A check box also exists to detail if approvals are automated or not.

Once the original 'Request for Change' form has been submitted the process checks to see if
1. this is a normal change
2. we are set to automatically manage approvals
3. the change is in an approval status

If the above conditions are true the system will identify the selected approval groups for the respective status and send a notification requesting approval.
Recipients of the approval notification can 'Approve' or 'decline' the request.  Each response option allows for comments to be added after the response has been sent.
If the response is positive, i.e. approved, the system checks to see if there are any subsequent approval stages defined and forwards a new notification to that set of defined approver group(s).
The system continues this automated process until such time as there are no subsequent approval stages or until we receive a 'Decline' response.

All comments submitted from each approval event are written back to the original 'Request for Change' event so the change manager can quickly see responses from each approval stage.

Once all approval stages are complete the change manager can manually duplicate the original 'Request for Change' event and progress the change through the remaining status.

If the original 'Request for Change' event is not configured for auto-approval the change manager can progress the change through each necessary status via manually duplicating the event a selecting the relevant status.

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
