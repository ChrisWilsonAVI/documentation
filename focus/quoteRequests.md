# Quote Requests Meeting

Requests separate into three work flows:

1. Quote Requests - Initial high level proposal with equipment list and functional scope only
1. Design Packs - Detailed design following on from client acceptance of the equipment list and functional scope
1. Variations - Post design pack changes to the project. Out of scope for this conversation

## Workflow

1. A Task is created against a Salesforce Opportunity
   - Subject = Quote Request
   - Status = Not Started
   - Due Date
   - Comments
   - Assigned To = UK House
   - Priority
1. Dashboard / Report created to show 'unassigned' tasks
1. Design Engineer assigns themselves to the task
   - Status = In Progress
   - Potential: workflow from Design Engineer 'completing' their task to creating a task for sales admin
   - Potential: indicate work waiting on others. Status = Waiting on someone else, Deferred, On Hold

## Report Requirements

- Determine report format for:
  - Unassigned Queue
    - Fields
      - Task
      - Client Name
      - Opportunity Name
      - Sector / Industry
      - Opportunity Type (Integration, Tender, Inside Sales)
      - Date Created / Duration
      - Due Date
      - Priority
      - Opportunity Close Date
      - Est. Project Start Date (?)
  - Dashboard
    - AM
    - Sector
    - Country
    - Fields
      - Task
      - Assigned
      - Status
      - Client Name
      - Opportunity Name
      - Sector / Industry
      - Opportunity Type (Integration, Tender, Inside Sales)
      - Date Created / Duration
      - Due Date
      - Priority
      - Opportunity Close Date
      - Est. Project Start Date (?)
  - Analysis
    - no. quote requests
    - duration
- Add new 'Opportunity Type' of Inside Sales

## Design Pack

1. When opportunity reaches 'Verbal' add event trigger to add row to SmartSheets

- Opportunity Number
- Account Manager
- Design Engineer
- Sales Admin
- Populate dates based on Est. Project Start Dates & Close Date in SF

1. Update of information handled outside of AX and Salesforce. After initial push of information no additional information is sent from SF.

### Follow Ups

- Question:
  - If we are looking to amend the process so that a project number is created when the opportunity reaches verbal, does this process/workflow still make sense?
