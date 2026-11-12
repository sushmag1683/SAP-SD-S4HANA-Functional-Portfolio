
# SAP S/4HANA – Sales Document Configuration

## 1. Objective

To understand sales document configuration and processing in SAP Sales and Distribution (SD).

## 2. Sales Document Types

Sales document types define the characteristics and processing rules of sales transactions.

Common examples:

| Document Type | Description |
|---|---|
| IN | Inquiry |
| QT | Quotation |
| OR | Standard Order |
| ZOR | Custom Sales Order |

## 3. Important Transaction Codes

| T-Code | Purpose |
|---|---|
| VOV8 | Define Sales Document Types |
| VOV7 | Define Item Categories |
| VOV4 | Assign Item Categories |
| VOV6 | Define Schedule Line Categories |
| VOV5 | Assign Schedule Line Categories |
| VA11 | Create Inquiry |
| VA21 | Create Quotation |
| VA01 | Create Sales Order |
| VA02 | Change Sales Order |
| VA03 | Display Sales Order |

## 4. Item Category Configuration

Item categories control how individual items are processed in a sales document.

Configuration activities:
- Define item categories.
- Maintain item category determination.
- Understand item category controls.

## 5. Schedule Line Category Configuration

Schedule line categories control delivery-related details such as:
- Delivery relevance
- Availability check
- Requirements transfer
- Movement type

## 6. Configuration and Determination

Document the following activities:

- Sales document type configuration.
- Item category configuration.
- Item category determination.
- Schedule line category configuration.
- Schedule line determination.

## 7. Practical Configuration Examples

Document custom configuration examples from the practice environment:

- Custom sales document types: ZOR, SOR and ZSOR.
- Custom item category: SAN.
- Custom schedule line category: ZP.

Include configuration screenshots and explain the purpose of each setting.

## 8. Testing and Validation

- Practised inquiry and quotation creation.
- Created sales orders using configured document types.
- Verified item category determination.
- Checked schedule line determination.
- Validated sales document processing.

## 9. Key Learning Outcomes

- Understood sales document configuration.
- Learned item category determination.
- Understood schedule line category controls.
- Practised sales document creation and validation.
