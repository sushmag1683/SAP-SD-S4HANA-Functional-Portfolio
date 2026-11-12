
# SAP S/4HANA – Shipping and Delivery Configuration

## 1. Objective

To understand shipping configuration and outbound delivery processing in SAP Sales and Distribution (SD).

## 2. Shipping Overview

Shipping activities manage the movement of goods from the supplying plant to the customer.

Key activities:
- Shipping point determination
- Outbound delivery creation
- Picking
- Post Goods Issue (PGI)
- Delivery monitoring

## 3. Important Organizational Elements

| Element | Description |
|---|---|
| Plant | Supplies materials for delivery |
| Storage Location | Identifies the storage area |
| Shipping Point | Responsible for processing deliveries |
| Loading Group | Represents the material's loading requirements |
| Shipping Condition | Represents customer or order shipping requirements |

## 4. Important Transaction Codes

| T-Code | Purpose |
|---|---|
| OVXD | Define Shipping Points |
| OVL2 | Assign Shipping Points |
| VL01N | Create Outbound Delivery |
| VL02N | Change Outbound Delivery |
| VL03N | Display Outbound Delivery |
| VL06O | Outbound Delivery Monitor |
| VL09 | Reverse Goods Issue |

## 5. Shipping Point Determination

Shipping point determination identifies the shipping point responsible for processing an outbound delivery.

It is based on:
- Shipping Condition
- Loading Group
- Delivering Plant

Configuration activities:
- Define shipping points.
- Maintain shipping point determination.
- Assign shipping points to plants.

## 6. Outbound Delivery Processing

Outbound delivery processing includes:

1. Create outbound delivery.
2. Check delivery quantities.
3. Perform picking where applicable.
4. Verify delivery details.
5. Execute Post Goods Issue (PGI).

## 7. Post Goods Issue (PGI)

PGI confirms that goods have been issued from inventory for delivery.

Key impacts:
- Inventory quantity is reduced.
- Material document is generated.
- Relevant accounting impact is posted, depending on the scenario and valuation settings.

## 8. Practical Learning

Document shipping configuration and delivery activities practised in the SAP S/4HANA practice environment.

## 9. Testing and Validation

- Verified shipping point determination where practised.
- Created outbound deliveries.
- Checked delivery quantities.
- Practised PGI execution where applicable.
- Reviewed delivery document flow.

## 10. Key Learning Outcomes

- Understood shipping point determination.
- Learned outbound delivery processing.
- Understood picking and PGI.
- Gained familiarity with shipping activities in SAP SD.

## 11. Screenshots

Configuration and testing screenshots are maintained in the Screenshots folder.
