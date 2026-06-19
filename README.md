# JobApplicationTracker (Zapier Automation)

## Overview
A Zapier workflow that automatically logs job applications to Google Sheets 
when a Google Form is submitted, eliminating manual data entry.

## How It Works
1. Applicant submits Google Form
2. Zapier trigger detects new form response
3. Data is mapped and transferred to a Google Sheets log
4. Email with Job Application info is sent to user

## Problem Solved
During development, I diagnosed and resolved failed field mappings that caused 
submission data to pass through empty. Fixed it by replacing the manually typed 
placeholder variables with Zapier's built-in field picker to correctly map 
form responses to their destination columns.

## Designed For Extensibility
Modular structure allows adding steps (email notifications, status tracking, 
reporting) without rebuilding the integration.

## Tools Used
- Zapier
- Google Forms
- Google Sheets
- Gmail
