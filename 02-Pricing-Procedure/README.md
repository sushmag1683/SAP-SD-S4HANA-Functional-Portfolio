
# SAP S/4HANA – Pricing Procedure Configuration

## 1. Objective
To understand the pricing determination process in SAP Sales and Distribution (SD).

## 2. Pricing Components

- Condition Tables
- Access Sequences
- Condition Types
- Pricing Procedures
- Condition Records
- Pricing Procedure Determination

## 3. Important Transaction Codes

| T-Code | Purpose |
|---|---|
| V/03 | Define Condition Tables |
| V/06 | Define Condition Types |
| V/07 | Define Access Sequences |
| V/08 | Define Pricing Procedures |
| OVKK | Determine Pricing Procedure |
| VK11 | Create Condition Records |
| VK12 | Change Condition Records |
| VK13 | Display Condition Records |

## 4. Condition Types

| Condition Type | Description |
|---|---|
| PR00 | Standard Base Price |
| K005 | Customer Discount |
| ZPR0 | Custom Base Price |
| ZD01 | Percentage Discount |
| ZD02 | Absolute Discount |
| ZFRA | Freight Surcharge |

## 5. Pricing Procedure Configuration

Document the following:
- Creation of condition types
- Assignment of access sequences
- Pricing procedure maintenance
- Step and counter configuration
- Pricing procedure determination
- Condition record maintenance

## 6. Pricing Scales

Document practical examples of:
- Base price scales
- Percentage discount scales
- Absolute discount scales
- Freight surcharge scales

## 7. Testing

Validate pricing determination in a sales order and document the expected and actual condition values.

## 8. Key Learning Outcomes

Summarize how condition techniques determine prices, discounts and surcharges in SAP SD.


## 9. Practical Configuration Example

The following custom condition types were practised in the SAP S/4HANA practice environment.

| Condition Type | Description | Purpose |
|---|---|---|
| ZPR0 | Z Base Price | Defines the base selling price |
| ZD01 | Z Percentage Discount | Applies percentage-based discounts |
| ZD02 | Z Absolute Discount | Applies fixed-value discounts |
| ZFRA | Z Freight Surcharge | Adds freight charges |

## 10. Pricing Procedure Determination

Pricing procedure determination depends on:

- Sales Area
- Document Pricing Procedure
- Customer Pricing Procedure

Transaction Code: OVKK

## 11. Testing and Validation

- Created condition records using VK11.
- Tested pricing determination in sales orders.
- Verified base price, discounts and freight conditions.
- Checked the determined pricing procedure.

## 12. Key Learning Outcomes

- Understood the condition technique in SAP SD.
- Practised creating custom condition types.
- Learned pricing procedure determination.
- Validated pricing conditions in sales documents.

