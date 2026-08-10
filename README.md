# AI Email Processing System

An end-to-end AI-powered email processing automation built with **UiPath, OpenAI API, Gmail, and PostgreSQL**.

The system automatically processes today's unread emails, uses AI to analyze and classify their content, extracts structured information, and stores the processed results in a PostgreSQL database.

## Contents

- [Business Problem](#business-problem)
- [How It Works](#how-it-works)
- [Demo](#demo)
- [Project Screenshots](#project-screenshots)
- [PostgreSQL Results](#postgresql-results)
- [Key Features](#key-features)
- [Technologies & Skills](#technologies--skills)
- [Automation Workflow](#automation-workflow)
- [Security](#security)
- [What I Learned](#what-i-learned)

---

## Business Problem

Businesses can receive large volumes of emails that require manual review, categorization, prioritization, and routing.

This project demonstrates how **AI and workflow automation** can transform unstructured email content into structured, actionable business data while reducing repetitive manual processing.

---

## How It Works

**Gmail Inbox**  
↓  
**Today's Unread Emails**  
↓  
**UiPath Automation**  
↓  
**OpenAI API Analysis**  
↓  
**Category + Priority + Department + Summary**  
↓  
**PostgreSQL Database**  
↓  
**Processing Summary**

---

## Key Features

- Processes today's unread Gmail messages
- Automatically reads email subject and body
- Sends email content to the OpenAI API for analysis
- Determines the email category
- Assigns a priority level
- Identifies the appropriate department
- Generates a concise email summary
- Converts the AI response into structured JSON data
- Stores processed email information in PostgreSQL
- Tracks the number of successfully processed emails
- Displays a final processing summary
- Reduces repeated processing by working with unread emails

---

## Complete UiPath Workflow

The workflow connects Gmail, UiPath, OpenAI, JSON processing, and PostgreSQL into one end-to-end automation.
<img width="941" height="1672" alt="ai-email-processing-workflow" src="https://github.com/user-attachments/assets/98599818-faea-4155-88a7-a56f1da981ec" />


![AI Email Processing System - UiPath Workflow](ai-email-processing-workflow.png)

---

## AI-Generated Output

For each processed email, the AI returns structured information such as:

| Field | Example |
|---|---|
| Category | Customer Complaint |
| Priority | High |
| Department | Customer Support |
| Summary | Customer reports an issue requiring urgent assistance. |

---

## PostgreSQL Results

After AI analysis, the structured email information is automatically stored in PostgreSQL.

The database stores:

- Sender
- Subject
- Category
- Priority
- Department
- AI-generated summary
- Processing status
- Processing date/time


https://github.com/user-attachments/assets/a8f0ecec-0e83-4f92-a31c-eb69a1d553da



https://github.com/user-attachments/assets/55e2ac4f-75f9-4232-bdd7-107863420ab5

<img width="2284" height="1878" alt="postgresql-results-github" src="https://github.com/user-attachments/assets/e1c73f9d-8d2e-4ef2-9b67-bb1158d25198" />

![PostgreSQL Processed Email Results](postgresql-processed-email-results.png)

---

## Technologies and Skills

| Technology | Use |
|---|---|
| **UiPath** | End-to-end workflow automation |
| **OpenAI API** | AI-powered email analysis and classification |
| **Gmail** | Email input and processing |
| **REST API** | Communication between UiPath and OpenAI |
| **PostgreSQL** | Structured data storage |
| **SQL** | Database operations |
| **JSON** | Structured AI response processing |
| **ODBC** | UiPath-to-PostgreSQL database connectivity |

---

## Automation Workflow

1. Process Today's Unread Emails
2. Get Email Subject
3. Get Email Body
4. Build OpenAI Request
5. Analyze Email with OpenAI
6. Extract AI Response Content
7. Clean AI Response
8. Parse AI Classification JSON
9. Extract Email Category
10. Extract Priority Level
11. Extract Email Summary
12. Extract Target Department
13. Save Email to PostgreSQL
14. Increment Processed Email Count
15. Show Processing Summary

---

## Demo Video

Watch the end-to-end automation in action:

**Gmail → UiPath → OpenAI API → AI Classification → PostgreSQL → Processing Summary**

### [▶ Watch the AI Email Processing System Demo](AI-Email-Processing-System-Demo-GitHub.mp4)

The demo shows the workflow processing emails, using AI to classify their content, and storing the structured results in PostgreSQL.

---

## What I Learned

Through this project, I gained practical experience in:

- Designing an end-to-end automation workflow
- Integrating UiPath with REST APIs
- Working with the OpenAI API
- Processing and parsing JSON responses
- Integrating Gmail with UiPath
- Connecting UiPath to PostgreSQL through ODBC
- Working with SQL and relational databases
- Transforming unstructured email content into structured data
- Building AI automation around a practical business use case

---

## Security

API keys, database passwords, and other confidential credentials are not shown in the screenshots or demo materials.

The public repository is intended to demonstrate the architecture, workflow, implementation, and results without exposing confidential credentials.

---

## Future Improvements

Possible future improvements include:

- Automatic department routing
- Automated email replies
- Stronger duplicate detection using Gmail message IDs
- Error handling and retry mechanisms
- Daily processing reports
- Analytics dashboard
- UiPath Orchestrator deployment

---

## Author

**Mohammad Jahidul Islam**

Automation & AI Automation Developer

Building practical automation solutions using **UiPath, APIs, AI, SQL, and databases**.
