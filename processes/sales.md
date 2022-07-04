[< Integration Process](./processes/integration.md)

# Sales Process

## Opportunity Stages

1. Identified
2. Qualified
3. Quoted
4. Verbal
5. Commit
6. Closed Won

## 01 - Identified

An identified opportunity is the initial stage of an opportunity. The opportunity is created when an account manager becomes aware of an upcoming business opportunity for a client. At this stage there is no requirement for understanding of specifics or value size.

**If the opportunity is for a new client, the new client process should be started prior to creating the opportunity.**

### Required Information

The account manager is responsible for adding the following information to the Salesforce opportunity

- Stage = "Identified Opportunity"
- Opportunity Name \*
- Account Name
- Main Contact
- Close Date
- Installing Office
- Est. Installation Date
- Booking by Region

* The opportunity name should be formatted in the following format:

`<Opportunity Number> - <Account Name>, <Project Reference>`

e.g. 123456 - ABC Widgets, London Boardroom Upgrade

## 02 - Qualified

An opportunity is qualified when a client's requirements have been been captured and we are in a position to produce a proposal. At this stage it will be determined who will be producing the proposal based on the opportunity type and location.

### Required Information

The account manager is responsible for adding the following information to the Salesforce opportunity

- Stage = "Qualified Opportunity"
- Opportunity Type
- Installation Location City
- Installation Location Country

### Defining Opportunity Type

**TODO: Define the different opportunity types**

### Opportunity Type - Box Sale

If the opportunity is for the supply of hardware only, then it will be classified as a Box Sale.

The account manager or sales admin will then create an opportunity folder on the M drive of their local office. The folder will be created with the following naming convention
`<Opportunity Number> - <Account Name>, <Project Reference>`

e.g. 123456 - ABC Widgets, London Boardroom Upgrade

**TODO: More information on the location of the opportunity folder**

A box sale proposal will be created by the account manager and sales admin and stored in the following folders on the M Drive:

- "02 - Proposal-SOW-Estimate Template"
  - Bill of Materials
  - Box sale proposal
- "14 - Special Pricing and Customer Quotes"
  - Supplier Quotes

### Integration Project

If the opportunity required hardware to be integrated, then it will be classified as an integration project.

The account manager or sales admin will then create an opportunity folder on the M drive of their local office. The folder will be created with the following naming convention:

`<Opportunity Number> - <Account Name>, <Project Reference>`

e.g. 123456 - ABC Widgets, London Boardroom Upgrade

Once the opportunity stage has been set to "Qualified Opportunity", it should enter the DE queue - However, the account manager will then also send an email to their design engineer requesting a proposal be created for this opportunity. The email will contain hyperlinks to both the Salesforce opportunity and the M: Drive opportunity folder.

Any information relating to the opportunity will be stored on the M drive in the following folders:

- "00 - Bid Documents"
  - Room standards
  - Touch panel layouts
- "01 - Site Survey Info"
  - Site Survey Forms
  - Pictures
  - Floor Plans

A bill of materials (BoM) will be created by the Design Engineer and stored in the following folders:

- "02 - Proposal-SOW Estimate Template"
  - Bill of Materials
  - Integration Proposal
- "13 - Subcontractor Quotes"
  - Quotes from local installation partners such as Vega
- "14 - Special Pricing and Customer Quotes"
  - Supplier Quotes

This is then sent onto the account manager and sales administrator to begin pricing.

The sales admin will price all items. A design engineer can occasionally request pricing from a vendor for bespoke items, however the responsibility for pricing accuracy sits with the sales admin.

**TODO: Add Link to detailed quoting process section**

[Quoting Process](./processes/quoting.md)

**TODO: Include Tender, Service, Renewal processes**
**TODO: update item categories in BoM to match AX**

## 03 - Quoted

An opportunity is quoted once the quote has been produced and the relevant checks and approvals have been completed.

Once the proposal is completed an email is sent, by the sales admin, to UK.approvals@avispl.com, for opportunities created by the UK office.

**See quoted approval process section for further details**

### Revisions

The opportunity remains at quoted until the client is happy with the design. Any revisions to the proposal following initial checks will need to be resubmitted to uk.approvals@avispl.com stating what changes have been made.

With every quote change, the sales admin team must update the sales figures on salesforce so that they accurately represent the latest version of the proposal.

### Version Control

When revising a proposal, the design engineer should first copy the latest version of the proposal into the active folder within the proposal folder "02-Proposal-SOW-Estimate/Archive" and then rename the file in the main folder:

`<Opportunity Number>-<Revision Number> - <Account Name>, <Project Reference>`
e.g. 123456-2 - ABC Widgets, London Boardroom Upgrade

## 04 - Verbal

The account manager will transfer the opportunity to verbal when the client has confirmed that the proposal doesn't require any further revisions and AVI-SPL will be awarded the work, but it is not known when the purchase orders will be received.

## 05 - Commit

The account manager will transfer the opportunity to commit when the client has confirmed that AVI-SPL will receive the purchase order and it is known when the purchase orders will be received.

## 06 - Closed

Upon receipt of a purchase order from the client an email should be sent to the sales admin of the installing office including:

- Client purchase order
- Link to M drive
- Link to Salesforce

At this time there should only be one version of the BoM and Proposal in the main section of "02 - Proposal-SOW Estimate Template" and all supplier quotes must be in folder 14 and up to date.

The sales admin will then check all information is correct and send the opportunity through to New Orders **See processing an order section**

The finance team will close the opportunity as won when the order has been processed.

### International Opportunity

**Move the international opportunities process to a separate workflow**

If, once the opportunity has been qualified, it is discovered that the installation is due to take place out of region, the opportunity needs to be sent to the Sales Manager within the region. The Sales Manager will assign a local account manager to support the opportunity from this point forward. This is done via the IQR process.

The account manager will then transfer the opportunity to the local account manager. The local account manager will then be referred to as the account manager for the rest of the process.

## Work Prioritisation

### Sales Admin

1. Processing Orders - This is essential on the last day of the month, as our accounts close on that day and all orders need to have projects associated to them.
2. Quoting a Variation
3. Net New Business
4. Other Admin Duties

## New Client Process

**TODO: Create new Account Setup Form**

If the opportunity is for a new client, due to access rights within Salesforce, the account manager will need to work with Sales Admin to create a new client by providing the team with the following information:

- Company Name
- Phone
- Email
- Website
- Company Address
  - Street
  - City
  - State
  - Postcode
  - Country
- Lead Source
- Industry
