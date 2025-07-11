OUTCOME:

successfully developed a smart, automated system that:

Detects and identifies products in real-time using YOLOv8 object detection.

Verifies product metadata including RoHS compliance, batch ID, and device ID.

Automatically generates a label with:

Product Name

Serial Number (unique & product-specific)

Manufacturing Date

Device ID & Batch ID

RoHS Compliance

Additional info (e.g., Warranty, Voltage, Storage, Supplier details)

QR Code containing all metadata

Logs all traceability data (product + label + timestamp + operator ID + shift) into a CSV file for audit and future trace.

LIMITATION:

 Limited Product Categories:
 
The current YOLOv8 model is trained only on a few product types (e.g., Remote, Lamp, Hard Disk).

It may not generalize well to new or unseen products without retraining.

Offline System:

No cloud-based storage or real-time remote monitoring.

Data is logged only locally (CSV); integration with cloud/database is not implemented.

SCOPE:

 Real-Time Product Detection:
Detect multiple product types using a trained YOLOv8 object detection model.

AI-Based Label Generation:
Auto-generates labels with product metadata, serial numbers, RoHS compliance, and more.


QR Code Integration:
Encodes full product metadata (ID, batch, manufacture date, RoHS, warranty, etc.) into scannable QR codes.

Traceability Logging:
Stores all product and label data (including timestamps, operator ID, shift, etc.) in a CSV log file.

Allows filtering by Device ID, Batch ID, Manufacturing Date, Shift, or Operator ID.

Component & Supplier Mapping:
Logs internal components and suppliers for each product, supporting detailed traceability.

RoHS Compliance Check:
Confirms product compliance with RoHS via pre-set metadata flags
