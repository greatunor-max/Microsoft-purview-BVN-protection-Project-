# Microsoft-purview-BVN-protection-Project-
Microsoft Purview project for Nigerian BVN detection, sensitivity labeling, and DLP protection.

## Overview

This project demonstrates how to use Microsoft Purview to protect sensitive Nigerian BVN data by:

- Creating a custom Sensitive Information Type (SIT)
- Applying Sensitivity Labels automatically
- Configuring DLP Policies
- Restricting Microsoft 365 Copilot from processing BVN data

---

# Technologies Used

- Microsoft Purview
- Microsoft 365
- Microsoft 365 Copilot
- DLP Policies
- Sensitivity Labels
- Regex

---

# Step 1 — Sensitive Information Type (SIT)

## SIT Name
Finance - Nigerian BVN

## Description
Detects Nigerian Bank Verification Numbers (BVN) in Microsoft 365 services.

## Regex Used

```regex
\b\d{11}\b
```

## Supporting Keywords
- BVN
- Bank Verification Number
- Nigerian BVN

---

# Step 2 — Sensitivity Label

## Label Name
Finance Confidential - BVN

The label automatically applies when BVN information is detected.

---

# Step 3 — DLP Policy

## Policy Name
Block Copilot Access to BVN Data

## Purpose
Prevent Microsoft 365 Copilot and Microsoft 365 services from processing or exposing BVN information.

---

# Step 4 — Testing

## Sample Test Data

```txt
Name: Unor Boliva
BVN: 22345678905
```

