# AI-Powered Email Management Agent

## Project Name
AI-Powered Email Management Agent

## Created With
- n8n
- Google Gemini AI
- Gmail Integration

## Purpose

This project is an AI-powered Email Management Agent designed to automate common email-related tasks.

The agent can interact with users through a chat interface, check recent emails, classify emails, add labels, and send emails based on user instructions.

---

# Logic Flow Breakdown

## 1. Chat Trigger

The workflow starts when a user enters a request through the chat interface.

Example:

> Send an email to someone@example.com.

The user can also ask the agent to check recent emails.

---

## 2. AI Agent

The AI Agent acts as the central controller of the workflow.

It understands the user's request and decides which action or Gmail tool should be used.

---

## 3. Gemini AI Model

Google Gemini acts as the intelligence component of the workflow.

It helps the AI Agent understand user requests and analyze email content.

The model is used to classify emails into:

- URGENT
- NORMAL
- SPAM

---

## 4. Gmail Tools

The AI Agent can use multiple Gmail tools.

### Get Recent Emails

Retrieves recent emails from the connected Gmail account.

### Send Email

Sends an email based on the user's instructions.

### Add Label

Adds labels to emails when required.

For example:

- URGENT emails can receive an URGENT label.
- SPAM emails can receive a SPAM label.

---

# Email Classification

Emails are classified into three categories:

### URGENT

Emails that require immediate attention or are time-sensitive.

### NORMAL

Legitimate emails that do not require immediate action.

### SPAM

Unwanted, suspicious, promotional, scam-like, or irrelevant emails.

---

# Tested Use Cases

### Sending Email

Input:

> Send an email to avimurkute.516@gmail.com with the subject "Test" and message "Testing Gmail connection."

The AI Agent uses the Gmail Send tool to send the email.

### Checking and Classifying Emails

The agent can retrieve recent emails and analyze their content using Gemini AI.

Based on the analysis, the email is classified as:

URGENT, NORMAL, or SPAM.

Appropriate labels can then be added automatically.

---

# Dependencies and Configuration

The following configuration is required:

- n8n instance (Self-hosted or Cloud)
- Google Gemini API credentials
- Gmail OAuth credentials
- Gmail account connected to n8n

---

# Future Improvements

- Add persistent memory for better conversation context.
- Add automatic email summarization.
- Add priority scoring for emails.
- Add notifications for urgent emails.
- Support multiple email accounts.
- Integrate additional communication platforms.

---

# Key Learning Outcomes

Through this project, I learned:

- How to build workflows using n8n.
- How AI Agents interact with external tools.
- How to connect Google Gemini with workflow automation.
- How to integrate Gmail tools with an AI Agent.
- How tool calling works in AI applications.
- How AI can perform actions beyond generating text.

---

## Workflow Overview

User Request

↓

Chat Trigger

↓

AI Agent

↓

Google Gemini AI

↓

Gmail Tools

├── Get Recent Emails

├── Send Email

└── Add Labels