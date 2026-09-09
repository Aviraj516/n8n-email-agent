# 📧 AI-Powered Email Management Agent

An AI-powered Email Management Agent built using **n8n, Google Gemini AI, and Gmail Integration**.

This project allows users to interact with an AI Agent through a chat interface and perform common email-related tasks such as checking emails, classifying emails, adding labels, and sending emails.

---

## 🚀 Features

- 📬 Check recent emails from Gmail
- 🧠 Classify emails as **URGENT, NORMAL, or SPAM**
- 🏷️ Automatically add labels based on email classification
- 📤 Send emails based on user instructions
- 💬 Interact with the agent through a chat interface
- 🤖 Use Gemini AI to understand requests and analyze email content
- ⚡ Allow the AI Agent to select the appropriate Gmail tool

---

## 🛠️ Technologies Used

- [n8n](https://n8n.io/)
- Google Gemini AI
- Gmail API / Gmail Integration
- AI Agent
- Workflow Automation

---

## 🧠 How It Works

The AI Agent acts as the central controller of the workflow.

It receives the user's request, understands the required action using Gemini AI, and selects the appropriate Gmail tool.

```text
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
```

---

## 📂 Email Classification

Emails are classified into three categories:

| Category | Description | Action |
|----------|-------------|--------|
| 🔴 URGENT | Requires immediate attention or is time-sensitive | Add URGENT label |
| 🟢 NORMAL | Legitimate email that does not require immediate action | No additional action |
| ⚠️ SPAM | Unwanted, suspicious, promotional, scam-like, or irrelevant | Add SPAM label |

---

## 💬 Example Prompts

### Send an Email

```text
Send an email to example@gmail.com with the subject "Meeting" and message "The meeting is scheduled at 5 PM."
```

### Check and Classify an Email

```text
Check my most recent email and classify it as URGENT, NORMAL, or SPAM.
```

---

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/Aviraj516/n8n-email-agent.git
cd n8n-email-agent
```

### 2. Import the Workflow

Open n8n and import:

```text
workflow/flow.json
```

### 3. Configure Credentials

You need to configure:

- Google Gemini API credentials
- Gmail OAuth credentials
- Gmail account permissions

> **Note:** Credentials and API keys are not included in this repository for security reasons.

### 4. Run the Workflow

Once the credentials are configured, activate or test the workflow through the n8n interface.

---

## 🧪 Tested Use Cases

### Email Sending

The AI Agent can understand a request such as:

```text
Send an email with a subject and message to a specified recipient.
```

The AI Agent automatically uses the Gmail Send tool to perform the action.

### Email Classification

The AI Agent can retrieve a recent email, analyze its content using Gemini AI, and classify it as:

- URGENT
- NORMAL
- SPAM

Based on the classification, the appropriate label can be added.

---

## 📁 Project Structure

```text
n8n-email-agent/
│
├── README.md
│
├── workflow/
│   └── flow.json
│
├── screenshots/
│
└── docs/
    └── Notes.pdf
```

---

## 🔮 Future Improvements

- Add persistent memory for conversation context
- Automatically summarize long emails
- Add priority scoring for emails
- Send notifications for urgent emails
- Support multiple email accounts
- Add calendar integration for meeting-related emails
- Create automatic replies for selected emails

---

## 📚 What I Learned

This project was my first hands-on project using **n8n**.

Through this project, I learned:

- How to build workflows using n8n
- How AI Agents interact with external tools
- How to integrate Google Gemini AI with workflow automation
- How Gmail tools can be connected to an AI Agent
- How AI tool calling works
- How AI can perform actions beyond generating text

---

## 📄 Documentation

Detailed project notes are available here:

[View Project Notes](docs/Notes.pdf)

---

## 👨‍💻 Author

**Aviraj Murkute**

---

⭐ If you found this project interesting, feel free to star the repository!