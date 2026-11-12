
# SAP S/4HANA – Billing and Copy Control

## 1. Objective

To understand billing document configuration and copy control in SAP Sales and Distribution (SD).

## 2. Billing Overview

Billing is an important stage of the Order-to-Cash process where invoices and other billing documents are generated.

Common billing scenarios:
- Order-related billing
- Delivery-related billing
- Credit memo
- Debit memo
- Returns-related credit memo

## 3. Important Transaction Codes

| T-Code | Purpose |
|---|---|
| VOFA | Define Billing Document Types |
| VOV7 | Define Item Categories |
| VTFA | Sales Document to Billing Document Copy Control |
| VTFL | Delivery to Billing Document Copy Control |
| VF01 | Create Billing Document |
| VF02 | Change Billing Document |
| VF03 | Display Billing Document |
| VF04 | Billing Due List |

## 4. Billing Document Types

Billing document types control the processing of billing transactions.

| Billing Type | Description |
|---|---|
| F1 | Order-Related Invoice |
| F2 | Delivery-Related Invoice |
| G2 | Credit Memo |
| L2 | Debit Memo |
| RE | Credit Memo for Returns |

## 5. Billing Relevance

Billing relevance determines how a sales document item is considered for billing.

Common concepts:
- Order-related billing
- Delivery-related billing
- Returns-related billing

## 6. Copy Control

Copy control defines how data is transferred from a preceding document to a subsequent document.

Important configuration areas:
- Source and target document types
- Header-level controls
- Item-level controls
- Copying requirements
- Data transfer routines
- Pricing type

## 7. Pricing Type in Copy Control

Pricing type determines how pricing conditions are handled when a subsequent document is created with reference to a preceding document.

Document the pricing types practised in the SAP environment and their effects on pricing redetermination.

## 8. Practical Learning

Document the following activities actually practised:

- Reviewed billing document types.
- Practised order-related billing configuration.
- Studied copy control settings.
- Understood the relationship between sales orders and billing documents.
- Reviewed pricing type settings.

## 9. Testing and Validation

Document the billing scenarios executed in the practice environment.

Include:
- Billing document creation.
- Billing value verification.
- Document flow verification.
- Accounting document checks, where performed.

## 10. Key Learning Outcomes

- Understood billing document processing.
- Learned billing relevance concepts.
- Understood copy control.
- Gained familiarity with pricing type settings.
- Understood billing integration with the O2C process.

## 11. Screenshots

Configuration and testing screenshots are maintained in the Screenshots folder.
