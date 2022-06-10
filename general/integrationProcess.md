# Integration Project Process

## Current Process

```mermaid
graph TB

    %%Styles
    classDef stage fill:#00205c,color:#E7E7E7,stroke-width:0;
    classDef process fill:#92C73A,color:#E7E7E7,stroke-width:0;

    %%Stages
    Lead[Lead]
    Demand([Demand Generation])
    Qualified(Qualified)
    Verbal(Verbal)
    Commit(Commit)
    OpportunityClose(Opportunity Closed)

    %%Processes
    Identified[Identified Opportunity]
    Identification([Identification])
    Quoting([Quoting])
    Quoted(Quoted)
    Revisions([Revisions])
    Design([Design Pack])
    Contract([Contract Negotiations])
    Processing([Order Processing])
    ProjectSetup([Project Setup])
    KickOff([Kick Off Meeting])
    EquipmentLoading([Equipment Loading])
    ResourceRequest([Resource Requests])
    Procurement([Equipment Ordering])
    GoodsIn([Equipment Received])
    %% RackFab([Rack Fabrication])
    %% WitnessTest([Witness Testing])
    GoodsOut([Equipment Sent to Site])
    Installation([Installation])
    Commissioning([Commissioning])
    %% ProgrammingOffsite([Offsite Programming])
    ClientHandover([Client Handover])
    InternalHandover([Handover to Service])
    Support([Support Contract Initiated])


    Lead-->Demand
    Demand --> Qualified

    Identified-->Identification
    Identification --> Qualified

    Qualified-->Quoting
    Quoting --> Quoted

    Quoted --> Revisions
    Revisions --> Verbal

    Verbal --> Design
    Design --> Commit
    Verbal --> Contract
    Contract --> Commit

    Commit --> Processing
    Processing --> ProjectSetup
    Processing --> OpportunityClose

    ProjectSetup --> KickOff
    KickOff --> EquipmentLoading
    KickOff --> ResourceRequest

    EquipmentLoading --> Procurement
    Procurement --> GoodsIn
    GoodsIn --> GoodsOut

    ResourceRequest --> Installation
    GoodsOut --> Installation

    Installation --> Commissioning
    Commissioning ---> ClientHandover
    Commissioning --> InternalHandover
    InternalHandover --> Support
```

## Notes

- Design Pack
  - Includes Scope of Works and M&E Drawings
  - Chargeable Effort
- Qualified
  - Consider different opportunity / project types
    - Service Only
    - RFP / Tender
    - Box Sale
- Quoting
  - Consider service involvement
- Proposed Change
  - Project created at verbal
