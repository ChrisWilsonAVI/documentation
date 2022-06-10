## Sales High Level

```mermaid
graph TB

    Lead
    Identified
    Qualified
    Quoted
    Verbal
    Commit


    Lead-->|Demand Generation|Qualified
    Identified-->|Qualification|Qualified
    Qualified-->|Quoting|Quoted
    Quoted-->|Revisions|Verbal
    Verbal-->|Design Pack & Contact Negotiation|Commit
    Commit-->|Order Processing|Closed[Closed Won]
```

## Quoting Process

Quoting process begins with a qualified opportunity where the Account Manager has booked a meeting with a client and a Design Engineer.

### Points to Consider

- Add in Service Quoting

```mermaid
sequenceDiagram
    participant Account Manager
    participant Design Engineer
    participant Sales Admin

    Note over Account Manager: Qualified Opportunity
    activate Account Manager
    Account Manager ->> Design Engineer: Opportunity Details Shared
    Note over Account Manager, Design Engineer: Initial Client Meeting
    Note over Design Engineer: Initial Design Created
    Design Engineer ->> Sales Admin: Designed BoM
    Note over Design Engineer: Create Technical Write Up
    Note over Sales Admin: Equipment Pricing
    Sales Admin ->> Design Engineer: Equipment Costed BoM
    Note over Design Engineer: Labour Calculated
    Design Engineer ->> Account Manager: Fully Costed BoM
    Note over Account Manager: Commercials Adjusted
    Note over Account Manager, Design Engineer: Approve Design and Commercials
    Design Engineer ->> Sales Admin: Approved Technical Write Up
    Note over Account Manager: Write Exec Summary
    Account Manager ->> Sales Admin: Exec Summary
    Account Manager ->> Sales Admin: Approved BoM
    Note over Sales Admin: Create Proposal
    Sales Admin ->> Account Manager: Completed Proposal
    Note over Sales Admin: Update Salesforce
    Note over Account Manager: Review Proposal with Client

```
