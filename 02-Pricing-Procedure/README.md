
# SAP S/4HANA – Enterprise Structure Configuration

## 1. Objective
To understand the organizational structure of SAP S/4HANA and its role in supporting Sales and Distribution (SD) business processes.

## 2. Organizational Units

| Organizational Unit | Description |
|---|---|
| Company Code | Represents an independent legal accounting entity |
| Sales Organization | Responsible for sales and distribution activities |
| Distribution Channel | Defines how products reach customers |
| Division | Represents a grouping of products or services |
| Plant | Organizational unit where materials are produced or stored |
| Storage Location | Identifies a specific storage area within a plant |
| Shipping Point | Organizational unit responsible for shipping deliveries |

## 3. Configuration Activities

- Define Company Code.
- Define Sales Organization.
- Define Distribution Channel.
- Define Division.
- Define Plant.
- Define Storage Location.
- Define Shipping Point.
- Assign organizational units according to SAP enterprise structure requirements.

## 4. Important Transaction Codes

| T-Code | Purpose |
|---|---|
| OX02 | Define Company Code |
| OVX5 | Define Sales Organization |
| OVXI | Define Distribution Channel |
| OVXB | Define Division |
| OX10 | Define Plant |
| OVL2 | Shipping Point Determination |

## 5. IMG Configuration Path

SPRO → SAP Reference IMG → Enterprise Structure

Configuration and assignment activities are available under the Definition and Assignment sections.

## 6. Integration with SAP SD

Enterprise structure supports:
- Sales document processing.
- Delivery processing.
- Shipping point determination.
- Billing and sales transactions.

## 7. Practical Learning

Practised creating and assigning enterprise structure components in an SAP S/4HANA practice environment.

## 8. Key Learning Outcomes

- Understood the relationship between organizational units.
- Learned how enterprise structure supports SAP SD processes.
- Practised organizational unit configuration and assignments.

