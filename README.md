# JobApplicationTracker (Zapier Automation)

## Overview
A Zapier workflow that automatically logs job applications to Google Sheets 
when a Google Form is submitted, eliminating manual data entry.
<img width="1323" height="810" alt="Image" src="https://github.com/user-attachments/assets/af9989dd-34c7-45f9-8ea5-49ddbf36d3f5" />

## How It Works
1. Applicant submits Google Form
<img width="1542" height="967" alt="Image" src="https://github.com/user-attachments/assets/0c24892e-7467-4760-8c02-82c713a232be" />

2. Zapier trigger detects new form response
3. Data is mapped and transferred to a Google Sheets log
<img width="785" height="797" alt="Image" src="https://github.com/user-attachments/assets/efde0502-e1ef-4713-a5e4-2f0ed6325b75" />

4. Confirmation email with Job Application info is sent to user
<img width="1601" height="401" alt="Image" src="https://github.com/user-attachments/assets/9755c099-6dbf-4350-92b3-0d98a8925393" />

## Problem Solved
During development, I diagnosed and resolved failed field mappings that caused 
submission data to pass through empty. Fixed it by replacing the manually typed 
placeholder variables with Zapier's built-in field picker to correctly map 
form responses to their destination columns.

## Designed For Extensibility
Modular structure allows adding steps ( status tracking, 
reporting dashboards or Slack notifications) without rebuilding the integration.

## Tools Used
- Zapier
- Google Forms
- Google Sheets
- Gmail
