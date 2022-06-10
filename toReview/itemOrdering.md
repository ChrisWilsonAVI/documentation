ITEM TYPES & CATEGORIES
This document details the definitions of item categories within AX and the correct loading and ordering of items.
CATEGORIES
The ‘Item’ item type has the following categories:
• EQUP – Item requirement category for any hardware lines to be ordered by AVI-SPL UK and installed by AVI-SPL UK. Each line must have an item number associated with it and be loaded through item requirements.
• SBCT – Procurement category for any items to be provided or charged by a partner or any hardware, consumables, or expense lines to be provided or charged by a subcontractor.
• SBCT-LAB – Item requirement category for any subcontractor labour. All lines should have one of the following item numbers:
o Project Management
o Site Management Days
o Project Engineer
o Rack Fabrication
o Installation Days
o Commissioning Days
o Programming Days
• WARR – Item requirement category for any renewable and non-renewable extended warranty items. Renewable extended warranty should only be ordered against an ‘06’ project. Each line must have an item number associated with it and be loaded through item requirements. Non-renewable extended warranty items these should only be ordered against an ‘01’ project. Each line must have an item number associated with it and be loaded through item requirements.
• LICENSE – Item requirement category for any software licenses. These should only be ordered against an ‘01’ project. Each line must have an item number associated with it and be loaded through item requirements.
• CONSUM – Procurement category for any consumables expense. To be posted to the ‘850X13-01’ project code only. Any consumables ordered to a project must be ordered as an EQUP item with an associated item number.
• FREIGHT – Procurement category for any costs associated with freight.
• PQTOTCOST – A Project finance category for monthly evaluations and financial adjustments. This should not be selected on a purchase order and should not be used without express permission from Project Finance.
• CREDIT – Procurement category for any line items showing refunds, credits, or discounts.
• HIRE – Procurement category for any physical equipment that is being hired for a project.
• CUSTOM – Procurement category for any one-off equipment lines such as a built-to-specification video wall or mounting plates.
Please note – Physical and Non-Physical items should not appear on the same purchase order. Please ensure that one order is raised containing any EQUP, CONSUM, FREIGHT, HIRE or CUSTOM lines and a second order is raised containing SBCT, SBCT-LAB, WARR, LICENSE.
CORRECT LOADING AND ORDERING
• Physical and Non-Physical items should not appear on the same purchase order. Please ensure that one order is raised containing any EQUP, CONSUM, FREIGHT, HIRE or CUSTOM lines and a second order is raised containing SBCT, SBCT-LAB, WARR, LICENSE.
• When an EQUP item is ordered it should only ever be ordered via the item requirements screen (and be evident on the engineering BOM). All ‘EQUP’ lines loaded are required to have an associated item number, sub-BOM (AV DRAWING ROOM REF noted on the current EBOM i.e. AV-001 etc.) and Room (if bespoke/tender) and mode of delivery e.g. site, rack.
• A reference number should be included with all purchase orders. This is the suppliers order reference number and will serve as a back-up reference if the suppliers delivery note does not reference our order number
• Consumables should only be ordered against the 850X13-01 project code. Any items to be ordered against a project should be loaded as either EQUP or CUSTOM
• The quantity ordered must match the quantity loaded through the item requirements screen (SalesQty).
• Items with a mode of delivery of ‘PM Hold’ must not be ordered under any circumstances. Only when the project manager advises an item can come off ‘PM Hold’ will the mode of delivery change and subsequent order raised.
ERRORS
The system will track the following errors:
• Delivery Date Missing – When an EQUP item is ordered through item requirements but does not have an est. delivery date. Only shown while items have an item status of ‘On Order’.
• Delivery Date Passed - When an EQUP item is ordered through item requirements and its est. delivery date has passed. Only shown while items have an item status of ‘On Order’.
• Item Number Missing – When an EQUP item is ordered without an item number being stated. Only shown prior to items having an item status of ‘Received’.
• Consumables costed to project – When an CONSUM item is ordered against a project other than the consumables project of ‘850X13-01’. Only shown prior to items having an item status of ‘Received’.
• Equipment not loaded correctly – When an EQUP item is not loaded through item requirements. Only shown prior to items having an item status of ‘Received’.
• Ordered while on Hold – Any item with a mode of delivery of ‘PM Hold’ where the qty ordered is not zero.
• Quantity ordered error – Any item that has been loaded through the item requirements screen where the quantity loaded does not equal the quantity loaded.
