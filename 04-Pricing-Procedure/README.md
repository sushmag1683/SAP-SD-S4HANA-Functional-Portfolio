
# SAP S/4HANA – Pricing Procedure Configuration

## 1. Objective

To understand the condition technique and pricing determination process in SAP Sales and Distribution (SD).

## 2. Pricing Condition Technique

The condition technique determines prices, discounts and surcharges in sales documents.

### Main Components

- Condition Tables
- Access Sequences
- Condition Types
- Pricing Procedures
- Condition Records

## 3. Important Transaction Codes

| T-Code | Purpose |
|---|---|
| V/03 | Define Condition Tables |
| V/06 | Define Condition Types |
| V/07 | Define Access Sequences |
| V/08 | Define Pricing Procedures |
| OVKK | Pricing Procedure Determination |
| VK11 | Create Condition Records |
| VK12 | Change Condition Records |
| VK13 | Display Condition Records |

## 4. Condition Types

Practised creating custom condition types in the SAP S/4HANA practice environment.

| Condition Type | Description | Purpose |
|---|---|---|
| ZPR0 | Z Base Price | Base selling price |
| ZD01 | Z Percentage Discount | Percentage-based discount |
| ZD02 | Z Absolute Discount | Fixed-value discount |
| ZFRA | Z Freight Surcharge | Freight charge |

## 5. Access Sequence Configuration

An access sequence determines the search strategy used to find valid condition records.

Configuration activities:
- Understand access sequence structure.
- Assign condition tables.
- Maintain access steps.
- Assign access sequences to condition types.

## 6. Pricing Procedure Configuration

Created a custom pricing procedure named ZPRC01.

Configuration activities:
- Maintain pricing procedure steps.
- Assign condition types.
- Maintain step and counter values.
- Configure subtotals and relevant controls.
- Verify pricing procedure determination.

## 7. Pricing Procedure Determination

Pricing procedure determination depends on:

- Sales Area
- Document Pricing Procedure
- Customer Pricing Procedure

**Transaction Code:** OVKK

## 8. Pricing Scales

Practised maintaining pricing scales for different condition types.

Examples:
- Base price scales.
- Percentage discount scales.
- Absolute discount scales.
- Freight surcharge scales.

## 9. Testing and Validation

- Created condition records using VK11.
- Tested pricing determination in sales orders.
- Verified base price and discount conditions.
- Checked freight surcharge conditions.
- Reviewed the determined pricing procedure.

## 10. Key Learning Outcomes

- Understood the condition technique.
- Practised custom condition type configuration.
- Learned access sequence and pricing procedure configuration.
- Understood pricing procedure determination.
- Validated pricing conditions in sales documents.

## 11. Screenshots

Configuration and testing screenshots are maintained in the Screenshots folder.
