
# SAP S/4HANA – Sales Document Configuration

## 1. Objective

To understand and configure sales document types, item categories and schedule line categories in SAP Sales and Distribution (SD).

## 2. Sales Document Types

Sales document types define how different sales transactions are processed in SAP SD.

### Common Sales Document Types

| Document Type | Description |
|---|---|
| IN | Inquiry |
| QT | Quotation |
| OR | Standard Order |
| RE | Returns |
| ZOR | Custom Sales Order |

### Configuration

- Define sales document types.
- Maintain document type controls.
- Configure number ranges and relevant document settings.
- Understand the role of sales document types in order processing.

**Transaction Code:** VOV8

## 3. Item Category Configuration

Item categories control how individual items behave within a sales document.

### Key Functions

- Controls item-level processing.
- Determines delivery relevance.
- Controls billing relevance.
- Influences pricing and other item-related settings.

**Transaction Codes:**
- VOV7 – Define Item Categories
- VOV4 – Assign Item Categories

## 4. Schedule Line Category Configuration

Schedule line categories control delivery and requirement-related activities for sales document items.

### Key Functions

- Delivery relevance
- Availability check
- Requirements transfer
- Movement type
- Schedule line processing

**Transaction Codes:**
- VOV6 – Define Schedule Line Categories
- VOV5 – Assign Schedule Line Categories

## 5. Practical Configuration Examples

The following custom configuration examples were practised in the SAP S/4HANA practice environment.

| Configuration | Custom Value |
|---|---|
| Sales Document Type | ZOR |
| Item Category | SAN |
| Schedule Line Category | ZP |

### Configuration Activities

- Created custom sales document types.
- Configured item category SAN.
- Created schedule line category ZP.
- Assigned schedule line category ZP to item category SAN.
- Verified determination during sales order creation.

## 6. Sales Document Processing

Important transaction codes used in sales document processing:

| T-Code | Purpose |
|---|---|
| VA11 | Create Inquiry |
| VA12 | Change Inquiry |
| VA13 | Display Inquiry |
| VA21 | Create Quotation |
| VA22 | Change Quotation |
| VA23 | Display Quotation |
| VA01 | Create Sales Order |
| VA02 | Change Sales Order |
| VA03 | Display Sales Order |

## 7. Testing and Validation

Practised the following activities:

- Created sales orders using configured document types.
- Checked item category determination.
- Verified schedule line category determination.
- Reviewed sales order item details.
- Validated the configuration through transaction execution.

## 8. Key Learning Outcomes

- Understood sales document type configuration.
- Learned item category determination.
- Understood schedule line category controls.
- Practised custom configuration and sales order validation.
- Gained knowledge of sales document processing in SAP S/4HANA.

## 9. Screenshots

Configuration and testing screenshots are maintained in the Screenshots folder.


