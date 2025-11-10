# AI Job Application Email Assistant (n8n + OpenAI)

An n8n workflow that automatically reads your job-related emails, detects whether they’re interview invitations, assessments, or rejections, and sends you instant study tips and prep checklists powered by GPT-4 mini.

## 🧠 How It Works
1. **Gmail Trigger** – watches your inbox for unread emails matching job keywords (assessment, interview, etc.).
2. **Text Classifier** – categorizes each message: assessment, interview, rejection, or other.
3. **AI Agent (GPT-4 mini)** – generates personalized prep tips for assessments and interviews.
4. **Gmail Send** – emails those tips to you (with `[JOB-PREP-BOT]` in the subject).
5. **Safety Filters** – ignores your own outgoing mails to prevent infinite loops.

## ⚙️ Setup
1. Run n8n (self-hosted or Cloud).
2. Add your Gmail credentials (OAuth2) and OpenAI API key.
3. Import `workflow.json`.
4. Update your email address and query in the **Gmail Trigger**:
