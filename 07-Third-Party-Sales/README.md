
# SAP S/4HANA – Third-Party Sales Process

## 1. Objective

To understand the third-party sales process in SAP SD and its integration with Materials Management (MM).

## 2. Process Overview

Third-party sales is a business process in which a company sells goods to a customer, but the goods are delivered directly by an external vendor to the customer.

The selling company does not physically handle the goods.

## 3. Business Process Flow

1. Customer places a sales order.
2. Sales order item is processed as a third-party item.
3. Purchase requisition is generated.
4. Purchasing team creates a purchase order.
5. Vendor delivers goods directly to the customer.
6. Vendor invoice is processed.
7. Customer billing is carried out according to the configured billing process.

## 4. Important Configuration Elements

| Element | Description |
|---|---|
| Item Category TAS | Standard third-party sales item category |
| Schedule Line Category CS | Standard third-party schedule line category |
| Purchase Requisition | Procurement requirement generated from the sales order |
| Purchase Order | Document used to procure goods from the vendor |

## 5. Important Transaction Codes

| T-Code | Purpose |
|---|---|
| VA01 | Create Sales Order |
| VA03 | Display Sales Order |
| ME51N | Create Purchase Requisition |
| ME53N | Display Purchase Requisition |
| ME21N | Create Purchase Order |
| ME23N | Display Purchase Order |
| MIGO | Goods Movement |
| MIRO | Enter Vendor Invoice |
| VF01 | Create Customer Billing Document |

## 6. SAP SD–MM Integration

Third-party sales involves integration between:

- SAP SD for sales order processing.
- SAP MM for procurement activities.
- SAP FI for relevant accounting postings.

## 7. Practical Learning

Document the third-party sales concepts and configuration activities practised in the SAP S/4HANA practice environment.

Include:
- Third-party item category.
- Schedule line category.
- Purchase requisition generation.
- Purchase order processing.
- Integration between sales and procurement.

## 8. Testing and Validation

Document the scenarios actually executed in the practice environment.

Verify:
- Third-party item category determination.
- Schedule line determination.
- Purchase requisition generation.
- Purchase order reference and document flow.

## 9. Key Learning Outcomes

- Understood third-party sales processing.
- Learned the integration between SAP SD and MM.
- Understood procurement document generation from sales requirements.
- Gained familiarity with vendor and customer document flows.

## 10. Screenshots

Configuration and testing screenshots are maintained in the Screenshots folder.
