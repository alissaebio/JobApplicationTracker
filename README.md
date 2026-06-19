# Job Application Tracker

## Overview
An automated workflow system built with Zapier that captures job application submissions, records them in Google Sheets, and sends confirmation emails without manual intervention.
<img width="1323" height="810" alt="Image" src="https://github.com/user-attachments/assets/af9989dd-34c7-45f9-8ea5-49ddbf36d3f5" />

## Architecture
Google Form → Zapier → Google Sheets → Gmail Confirmation

The workflow uses Google Forms as the data source, Zapier as the orchestration layer, Google Sheets as the system of record, and Gmail for automated user notifications.

## Outcomes

The workflow can:

- Automatically capture job application submissions
- Log application data without manual entry
- Send confirmation emails to applicants
- Maintain consistent records in Google Sheets
- Support future workflow extensions with minimal changes

## Key Skills Demonstrated

- Workflow Automation
- Zapier
- Integration Development
- Troubleshooting
- Business Process Automation
- Workflow Maintenance
- System Reliability
- Data Validation

## Design Decisions

Zapier was selected because it provides reliable event-driven automation and rapid integration between Google services without requiring custom infrastructure.
This approach reduced implementation complexity while remaining easy to maintain and extend.

## How It Works
1. Applicant submits Google Form
<img width="1542" height="967" alt="Image" src="https://github.com/user-attachments/assets/0c24892e-7467-4760-8c02-82c713a232be" />

2. Zapier trigger detects new form response
3. Data is mapped and transferred to a Google Sheets log
<img width="785" height="797" alt="Image" src="https://github.com/user-attachments/assets/efde0502-e1ef-4713-a5e4-2f0ed6325b75" />

4. Confirmation email with Job Application info is sent to user
<img width="1601" height="401" alt="Image" src="https://github.com/user-attachments/assets/9755c099-6dbf-4350-92b3-0d98a8925393" />

## Technical Challenges

### Field Mapping Failure

Submission data was arriving as blank values in Google Sheets.

**Root Cause:**
- Fields were manually entered rather than dynamically mapped.

**Solution:**
- Reconfigured Zapier mappings using form response variables from the trigger event.
- Validated end-to-end data flow through testing.

**Result:**
- Restored reliable automated transfer of form data.

## Designed For Extensibility
Modular structure allows adding steps (status tracking, 
reporting dashboards, or Slack notifications) without rebuilding the integration.

## Reliability Considerations

To improve workflow reliability, the integration was tested end-to-end to verify 
successful data transfer between Google Forms, Zapier, Google Sheets, and Gmail.

Validation included:

- Confirming form submissions were correctly mapped to destination fields
- Verifying data was written accurately to Google Sheets
- Testing automated email delivery after successful submissions
- Structuring the workflow to support future maintenance and expansion

## Tools Used
- Zapier
- Google Forms
- Google Sheets
- Gmail
