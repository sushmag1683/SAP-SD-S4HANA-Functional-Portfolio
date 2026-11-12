# 05 – Third-Party Sales | SAP S/4HANA SD

## 1. Overview

Third-Party Sales is a special sales process in SAP SD where the company receives a customer order but does not deliver the goods directly from its own inventory.

Instead, the company procures the goods from an external vendor, who delivers them directly to the customer.

This process integrates SAP Sales and Distribution (SD) with Materials Management (MM).

## 2. Business Scenario

A customer places an order for a product.

The company creates a sales order and SAP generates a purchase requisition for the required material.

The purchasing department converts the purchase requisition into a purchase order. The vendor delivers the goods directly to the customer.

The company then creates a customer billing document based on the relevant process configuration.

## 3. Third-Party Sales Process Flow

Customer Order  
↓  
Sales Order Creation  
↓  
Purchase Requisition Generation  
↓  
Purchase Order Creation  
↓  
Vendor Delivery to Customer  
↓  
Supplier Invoice Processing  
↓  
Customer Billing

## 4. Important Configuration Elements

### A. Item Category – TAS

TAS is the standard item category used for third-party sales.

It controls the processing of third-party sales order items.

**Transaction Code:** VOV7 – Define Item Categories.

### B. Schedule Line Category – CS

CS is the standard schedule line category commonly used for third-party sales.

It supports the generation of a purchase requisition based on the relevant configuration.

**Transaction Code:** VOV6 – Define Schedule Line Categories.

### C. Item Category Determination

Item category determination identifies the appropriate item category based on the sales document type, item category group, usage and higher-level item category.

**Transaction Code:** VOV4.

### D. Schedule Line Category Determination

Schedule line category determination identifies the appropriate schedule line category based on the item category and MRP type.

**Transaction Code:** VOV5.

## 5. Important Transaction Codes

| Transaction Code | Purpose |
|---|---|
| VA01 | Create Sales Order |
| VA03 | Display Sales Order |
| VOV4 | Item Category Determination |
| VOV5 | Schedule Line Category Determination |
| VOV6 | Define Schedule Line Categories |
| VOV7 | Define Item Categories |
| ME53N | Display Purchase Requisition |
| ME23N | Display Purchase Order |
| MIGO | Goods Movement |
| MIRO | Enter Supplier Invoice |
| VF01 | Create Customer Billing Document |
| VF03 | Display Billing Document |

## 6. Role of SD–MM Integration

Third-party sales demonstrates integration between Sales and Distribution and Materials Management.

- SD manages the customer sales order.
- MM manages purchasing activities.
- A purchase requisition can be generated from the sales order.
- Purchasing converts the requisition into a purchase order.
- The vendor delivers goods directly to the customer.

## 7. Practical Work and Verification

The following activities can be documented based on actual system execution:

- Understanding the third-party sales business process.
- Understanding item category TAS.
- Understanding schedule line category CS.
- Verifying purchase requisition generation.
- Tracking the relationship between sales and purchasing documents.

Only configurations and transactions actually performed in the practice system are presented as completed work.

## 8. Key Learnings

- Understanding third-party sales processing.
- Understanding item category TAS.
- Understanding schedule line category CS.
- Understanding automatic purchase requisition generation.
- Understanding SD–MM integration.
- Understanding vendor-to-customer direct delivery.

---

**Module:** SAP S/4HANA Sales and Distribution (SD)  
**Section:** Third-Party Sales  
**Project:** SAP SD Functional Configuration and Implementation Portfolio
