# 03 – Order-to-Cash (OTC) | SAP S/4HANA SD

## 1. Overview

Order-to-Cash (OTC) is an end-to-end business process in SAP Sales and Distribution (SD), starting with customer enquiries and ending with customer billing.

It covers pre-sales activities, sales order processing, delivery processing, goods issue and billing.

The objective of this process is to manage customer orders efficiently and ensure accurate sales and financial transactions.

## 2. Sales Document Types

Sales document types control how different sales transactions are processed in SAP SD.

### Important Sales Document Types

| Document Type | Description |
|---|---|
| IN | Inquiry |
| QT | Quotation |
| OR | Standard Order |
| ZOR | Custom Sales Order |
| RE | Returns |
| Custom Types | User-defined sales documents |

### Configuration

- Transaction Code: VOV8
- IMG Path: SPRO → Sales and Distribution → Sales → Sales Documents → Sales Document Header → Define Sales Document Types.

Important settings include:
- Sales document category
- Number range assignment
- Delivery and billing relevance
- Reference requirements
- Document controls

## 3. Inquiry Management

An inquiry is a pre-sales document used to record a customer's request for information about products, prices and availability.

### Process

- Create Inquiry – VA11
- Change Inquiry – VA12
- Display Inquiry – VA13

### Business Purpose

- Record customer requirements.
- Maintain requested materials and quantities.
- Provide a reference for quotation creation.

## 4. Quotation Management

A quotation is a formal offer provided to a customer based on the requested products, quantities, prices and validity period.

### Process

- Create Quotation – VA21
- Change Quotation – VA22
- Display Quotation – VA23

### Business Purpose

- Provide proposed prices to customers.
- Maintain quotation validity.
- Convert an accepted quotation into a sales order.

## 5. Sales Order Processing

A sales order is a commercial document created when a customer places an order for products or services.

### Process

- Create Sales Order – VA01
- Change Sales Order – VA02
- Display Sales Order – VA03

### Important Sales Order Information

- Sold-to Party
- Ship-to Party
- Bill-to Party
- Payer
- Material
- Order Quantity
- Plant
- Pricing Conditions
- Requested Delivery Date

### Important Concepts

- Sales document types
- Item categories
- Schedule line categories
- Partner determination
- Pricing determination
- Availability check
- Plant determination

## 6. Outbound Delivery

Outbound delivery is created to initiate the process of shipping goods to the customer.

### Process

- Create Outbound Delivery – VL01N
- Change Outbound Delivery – VL02N
- Display Outbound Delivery – VL03N

### Important Activities

- Delivery creation
- Picking
- Packing, where applicable
- Goods issue preparation

## 7. Picking and Post Goods Issue (PGI)

Picking is the process of selecting the required goods from the storage location to fulfil the customer order.

Post Goods Issue (PGI) confirms that the goods have been issued from the delivering plant.

### Transaction Codes

- VL02N – Change Outbound Delivery
- VL03N – Display Outbound Delivery

### Effects of PGI

- Reduces inventory.
- Updates stock quantities.
- Creates the relevant material document.
- Posts accounting entries where applicable.
- Updates delivery status.

## 8. Billing Process

Billing is the process of generating an invoice for the customer based on the relevant sales or delivery document.

### Transaction Codes

- VF01 – Create Billing Document
- VF02 – Change Billing Document
- VF03 – Display Billing Document

### Important Concepts

- Billing document types
- Order-related billing
- Delivery-related billing
- Pricing in billing
- Accounting document generation

## 9. Document Flow

Document Flow provides a connected view of the documents created throughout the OTC process.

It helps track the relationship and processing status of preceding and subsequent documents.

### Example Process Flow

Inquiry → Quotation → Sales Order → Outbound Delivery → Picking → PGI → Billing

### Transaction Code

VA03 – Display Sales Order → Environment → Document Flow.

## 10. Important IMG Configuration Paths

| Configuration | IMG Path |
|---|---|
| Sales Document Types | SPRO → Sales and Distribution → Sales → Sales Documents → Sales Document Header → Define Sales Document Types |
| Item Categories | SPRO → Sales and Distribution → Sales → Sales Documents → Sales Document Item → Define Item Categories |
| Schedule Line Categories | SPRO → Sales and Distribution → Sales → Sales Documents → Schedule Lines → Define Schedule Line Categories |

## 11. Practical Work and Verification

The practical activities covered in this section include:

- Understanding sales document types.
- Creating and displaying inquiries.
- Creating and displaying quotations.
- Creating and processing sales orders.
- Creating outbound deliveries.
- Performing picking and PGI.
- Creating and displaying billing documents.
- Verifying the complete document flow.

Only configurations and transactions actually performed in the practice system are presented as completed work.

## 12. Key Learnings

- Understanding the complete Order-to-Cash process.
- Difference between inquiry, quotation and sales order.
- Understanding sales document types and controls.
- Understanding delivery and goods issue processing.
- Understanding billing and accounting integration.
- Tracking documents using document flow.

---

**Module:** SAP S/4HANA Sales and Distribution (SD)  
**Section:** Order-to-Cash (OTC)  
**Project:** SAP SD Functional Configuration and Implementation Portfolio
