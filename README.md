## SafeStock-Clinical: Inventory Management with LASA Alerts
SafeStock-Clinical is a professional Python-based inventory tracking system designed specifically for medical environments. It bridges the gap between healthcare domain knowledge and software engineering to enhance patient safety and optimize supply chain management.

 Overview
In clinical settings, "Look-Alike Sound-Alike" (LASA) medications are a primary source of medication errors. This project implements a safety-first approach by integrating clinical risk alerts directly into the inventory workflow.

# Key Features
Smart Search: Quickly filter clinical supplies (e.g., Gloves, Syringes, Medications) by name with case-insensitive matching.

Clinical Safety Alerts: Real-time warnings for LASA medications to prevent selection errors before they reach the patient.

Stock Transaction Management: Automated stock reduction and real-time balance updates.

Low Stock Notification: Visual cues when an item drops below the predefined "Minimum Required" threshold.

Robust Error Handling: Integrated try-except blocks to manage invalid user inputs and prevent system crashes in high-pressure environments.

# Technical Stack
Language: Python 3.x

Library: Pandas (for high-performance data manipulation and CSV persistence)

Data Storage: CSV-based local database for easy portability.

# Data Architecture
The system operates on a structured clinic_inventory.csv database with the following attributes:
| Attribute | Description |
| :--- | :--- |
| Item_ID | Unique identifier for each clinical supply. |
| Item_Name | Full name and batch details of the product. |
| Category | Categorization (Medication, Consumable, Surgical). |
| Current_Stock | Real-time quantity available in the clinic. |
| LASA_Warning | Boolean flag (True/False) for high-risk medications. |

# How to Run
Ensure you have Python and Pandas installed.

Place your clinic_inventory.csv in the same directory as the script.

Execute the script:

Bash
python SafeStock_Clinical.ipynb
Follow the on-screen prompts to search, verify, and update inventory.

# About the Developer
Developed by a Nursing and Computer Programming student dedicated to advancing Health Informatics and digital transformation in clinical practice.
