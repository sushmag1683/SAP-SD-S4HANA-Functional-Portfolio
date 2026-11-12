# 02 – Master Data | SAP S/4HANA SD

## 1. Overview

Master Data is the foundation of SAP Sales and Distribution (SD). It contains essential information about customers and materials required to execute business transactions.

In SAP S/4HANA, Business Partner (BP) is the central approach for maintaining customer master data.

This section covers Business Partner, Customer Master Data and Material Master Data and explains their importance in the Order-to-Cash (OTC) process.

## 2. Business Partner (BP)

### Introduction

Business Partner is the central master data object in SAP S/4HANA used to maintain information about business entities such as customers and suppliers.

Customer-related information is maintained through appropriate BP roles.

### Important BP Roles

| BP Role | Description |
|---|---|
| FLCU00 | Customer – Financial Accounting |
| FLCU01 | Customer – Sales and Distribution |

### Business Partner Data Structure

**A. General Data**

General data is maintained at client level and can be shared across organizational units.

Important information:
- Business Partner Name
- Address
- Country and Region
- Communication Details
- Search Terms

**B. Company Code Data**

Company code data contains financial information specific to a company code.

Important information:
- Reconciliation Account
- Payment Terms
- Payment Methods
- Dunning Information
- Account Management Details

**C. Sales Area Data**

Sales area data contains customer information relevant to sales transactions.

A Sales Area consists of:

Sales Organization + Distribution Channel + Division

Important information:
- Sales District
- Currency
- Pricing Procedure Indicator
- Shipping Conditions
- Incoterms
- Delivering Plant

*Note: Sales Area Data is a separate customer data segment. Include its practical configuration only if it was maintained in your system.*

## 3. Customer Master Data

Customer Master Data stores information required for sales, delivery, billing and financial transactions.

### Three Main Data Segments

| Data Segment | Description |
|---|---|
| General Data | Customer information maintained at client level |
| Company Code Data | Financial information maintained for a company code |

### Customer Partner Functions

Partner functions identify the roles performed by different business partners in a sales transaction.

| Partner Function | Description |
|---|---|
| SP | Sold-to Party |
| SH | Ship-to Party |
| BP | Bill-to Party |
| PY | Payer |

These partner functions determine who places the order, receives the goods, receives the invoice and makes the payment.

## 4. Material Master Data

### Introduction

Material Master contains information about materials and products used throughout different business processes in SAP.

In SAP SD, material master data supports sales order processing, pricing, delivery and billing.

### Important Material Master Views

**A. Basic Data 1 and Basic Data 2**

Contains general material information.

Important fields:
- Material Description
- Base Unit of Measure
- Material Group
- Material Type
- Weight and Dimensions

**B. Sales: Sales Org. 1**

Contains sales-specific information.

Important fields:
- Sales Unit
- Delivering Plant
- Tax Classification
- Minimum Order Quantity
- Material Statistics Group

**C. Sales: Sales Org. 2**

Contains additional sales and accounting-related information.

Important fields:
- Material Pricing Group
- Account Assignment Group
- Item Category Group

**D. Sales: General/Plant**

Contains sales and plant-specific information.

Important fields:
- Availability Check
- Transportation Group
- Loading Group
- Profit Center

## 5. Important Transaction Codes

| Transaction Code | Purpose |
|---|---|
| BP | Maintain Business Partner |
| MM01 | Create Material |
| MM02 | Change Material |
| MM03 | Display Material |

## 6. Role of Master Data in Order-to-Cash

Customer and Material Master Data play an important role in the OTC process.

**Process Flow:**

Customer Master + Material Master  
↓  
Sales Order Creation (VA01)  
↓  
Pricing and Availability Checks  
↓  
Outbound Delivery  
↓  
Picking and Post Goods Issue  
↓  
Billing Document

### Business Importance

- Customer master provides customer and sales-related information.
- Material master provides product and sales-related information.
- Partner functions determine the roles of business partners.
- Material sales views support sales and delivery processing.
- Accurate master data helps ensure smooth sales transactions.

## 7. Practical Work and Verification

The following activities are covered as part of the SAP S/4HANA SD master data practice:

- Understanding Business Partner structure and roles.
- Exploring General Data and Company Code Data.
- Understanding customer partner functions.
- Exploring Material Master Basic Data.
- Understanding Material Master Sales Views.
- Identifying the master data required for sales order processing.

Only configurations and activities actually performed in the practice system are presented as completed work.

## 8. Key Learnings

- Understanding Business Partner in SAP S/4HANA.
- Difference between General Data, Company Code Data and Sales Area Data.
- Understanding customer partner functions.
- Understanding Material Master views relevant to SAP SD.
- Identifying the relationship between master data and OTC transactions.

---

**Module:** SAP S/4HANA Sales and Distribution (SD)  
**Section:** Master Data  
**Project:** SAP SD Functional Configuration and Implementation Portfolio
