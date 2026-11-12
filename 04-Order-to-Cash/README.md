
# SAP S/4HANA – Order-to-Cash (O2C) Process

## 1. Objective

To understand the end-to-end Order-to-Cash process in SAP S/4HANA Sales and Distribution.

## 2. O2C Process Overview

The Order-to-Cash process covers the activities from customer inquiry and sales order processing through delivery, goods issue and billing.

## 3. Process Flow

1. Inquiry
2. Quotation
3. Sales Order
4. Outbound Delivery
5. Picking
6. Post Goods Issue (PGI)
7. Billing
8. Accounting Document

## 4. Important Transaction Codes

| T-Code | Purpose |
|---|---|
| VA11 | Create Inquiry |
| VA21 | Create Quotation |
| VA01 | Create Sales Order |
| VA03 | Display Sales Order |
| VL01N | Create Outbound Delivery |
| VL02N | Change Outbound Delivery |
| VL03N | Display Outbound Delivery |
| VF01 | Create Billing Document |
| VF03 | Display Billing Document |

## 5. Key Process Activities

### Sales Order Processing
- Create sales orders.
- Verify customer and material details.
- Check pricing determination.
- Review schedule lines.

### Delivery Processing
- Create outbound delivery.
- Perform picking where applicable.
- Verify delivery quantities.

### Post Goods Issue
- Execute PGI.
- Understand inventory and goods movement impact.

### Billing
- Create billing documents.
- Verify billing values.
- Understand accounting integration.

## 6. Document Flow

Document the relationship between:
- Inquiry and quotation.
- Sales order and delivery.
- Delivery and goods issue.
- Sales order or delivery and billing.

## 7. Testing and Validation

Document the O2C scenarios actually executed in the SAP practice environment.

## 8. Key Learning Outcomes

- Understood the complete O2C lifecycle.
- Practised sales order and delivery processing.
- Executed PGI and billing.
- Understood document flow and integration concepts.
