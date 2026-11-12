
# 04 – Pricing Configuration | SAP S/4HANA SD

## 1. Overview

Pricing is an important functionality in SAP Sales and Distribution (SD) used to determine the selling price of products and services during sales transactions.

SAP uses the Condition Technique to determine prices, discounts, surcharges, freight and taxes based on predefined conditions and pricing procedures.

## 2. Condition Technique

Condition Technique is the mechanism used by SAP to determine pricing conditions automatically.

It consists of four major components:

1. Condition Tables
2. Access Sequences
3. Condition Types
4. Pricing Procedures

### Pricing Determination Flow

Condition Table → Access Sequence → Condition Type → Pricing Procedure → Pricing Result

## 3. Condition Tables

Condition tables define the key fields used to store and retrieve condition records.

Examples of key fields:
- Customer
- Material
- Sales Organization
- Distribution Channel

**Transaction Codes:**
- V/03 – Create Condition Table
- V/04 – Change Condition Table
- V/05 – Display Condition Table

## 4. Access Sequences

An access sequence defines the search strategy used by SAP to find valid condition records.

It contains one or more accesses to condition tables.

Important concepts:
- Access sequence
- Access numbers
- Condition tables
- Exclusive indicator

**Transaction Codes:**
- V/07 – Maintain Access Sequences

## 5. Condition Types

Condition types represent individual pricing elements in SAP.

Examples:
- PR00 – Base Price
- K004 – Material Discount
- KF00 – Freight
- MWST – Output Tax

### Custom Condition Types

The following custom condition types were configured in the practice system:

| Condition Type | Description |
|---|---|
| ZPR0 | Z Base Price |
| ZD01 | Z Percentage Discount |
| ZD02 | Z Absolute Discount |
| ZFRA | Z Freight Surcharge |

**Transaction Codes:**
- V/06 – Maintain Condition Types
- VK11 – Create Condition Records
- VK12 – Change Condition Records
- VK13 – Display Condition Records

## 6. Pricing Procedure

A pricing procedure determines the sequence in which pricing conditions are calculated in a sales transaction.

### Custom Pricing Procedure

Pricing Procedure: ZPRC01

Configured condition elements include:
- Base Price
- Percentage Discount
- Absolute Discount
- Freight Surcharge

Important pricing procedure fields:
- Step
- Counter
- Condition Type
- From/To
- Requirement
- Subtotal
- Statistical indicator

**Transaction Code:** V/08 – Define Pricing Procedures.

## 7. Pricing Procedure Determination

Pricing procedure determination identifies which pricing procedure should be used for a sales transaction.

It is based on three important elements:

1. Sales Area
2. Document Pricing Procedure
3. Customer Pricing Procedure

**Transaction Code:** OVKK – Determine Pricing Procedure.

## 8. Condition Records

Condition records store the actual values used by SAP during pricing determination.

Examples:
- Base selling price
- Customer discounts
- Material discounts
- Freight charges

**Transaction Codes:**
- VK11 – Create Condition Records
- VK12 – Change Condition Records
- VK13 – Display Condition Records

## 9. Pricing in Sales Order

During sales order creation, SAP determines the applicable pricing procedure and condition records.

**Transaction Code:** VA01 – Create Sales Order.

The pricing screen displays:
- Base Price
- Discounts
- Surcharges
- Freight
- Taxes, where applicable
- Net Value

## 10. Important IMG Paths

| Configuration | IMG Path |
|---|---|
| Condition Tables | SPRO → Sales and Distribution → Basic Functions → Pricing → Pricing Control → Define Condition Tables |
| Access Sequences | SPRO → Sales and Distribution → Basic Functions → Pricing → Pricing Control → Define Access Sequences |
| Condition Types | SPRO → Sales and Distribution → Basic Functions → Pricing → Pricing Control → Define Condition Types |
| Pricing Procedures | SPRO → Sales and Distribution → Basic Functions → Pricing → Pricing Control → Define and Assign Pricing Procedures |

## 11. Practical Work and Verification

The practical activities covered in this section include:

- Understanding the condition technique.
- Creating and maintaining condition tables.
- Configuring access sequences.
- Creating custom condition types.
- Configuring pricing procedure ZPRC01.
- Maintaining pricing procedure determination.
- Creating condition records.
- Verifying pricing results in sales orders.

Only configurations actually completed and verified in the practice system are presented as completed work.

## 12. Key Learnings

- Understanding SAP SD condition technique.
- Difference between condition tables and access sequences.
- Understanding condition types and their calculation methods.
- Configuring pricing procedures.
- Understanding pricing procedure determination.
- Verifying pricing conditions in sales orders.

---

**Module:** SAP S/4HANA Sales and Distribution (SD)  
**Section:** Pricing Configuration  
**Project:** SAP SD Functional Configuration and Implementation Portfolio
