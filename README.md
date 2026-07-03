# 📧 AI Multi-Agent Email Writer

An AI-powered **Multi-Agent Email Writer** built using the **OpenAI Agents SDK**, **Groq Llama 3.3**, and **Resend API**. The project demonstrates how multiple AI agents can collaborate to generate, evaluate, optimize, and automatically send high-quality cold sales emails.

Instead of relying on a single language model response, the system creates multiple email drafts with different writing styles, selects the strongest version, converts it into a professional HTML email, generates an engaging subject line, and sends it using the Resend email service.

---

## 🚀 Features

* 🤖 Multiple AI agents working together
* ✍️ Generates cold sales emails in different writing styles
* 🏆 Automatically selects the best email draft
* 📨 Generates an engaging subject line
* 🎨 Converts plain text into a professional HTML email
* 📤 Sends emails automatically using the Resend API
* ⚡ Uses Groq's Llama 3.3 model for fast inference
* 🔧 Built using the OpenAI Agents SDK

---

## 🛠 Tech Stack

| Technology              | Purpose                         |
| ----------------------- | ------------------------------- |
| Python                  | Backend                         |
| OpenAI Agents SDK       | Multi-agent orchestration       |
| Groq API                | LLM inference                   |
| Llama 3.3 70B Versatile | Language model                  |
| Resend API              | Email delivery                  |
| AsyncIO                 | Parallel agent execution        |
| Requests                | API communication               |
| dotenv                  | Environment variable management |

---

## 📂 Project Structure

```text
mail-writer/
│
├── mail_writer.ipynb
├── .env
├── requirements.txt
└── README.md
```

---

## 🧠 Agent Workflow

```text
                User Prompt
                     │
                     ▼
        ┌────────────────────────┐
        │ Sales Manager Agent    │
        └──────────┬─────────────┘
                   │
      ┌────────────┼─────────────┐
      ▼            ▼             ▼
 Professional   Engaging      Concise
 Sales Agent   Sales Agent   Sales Agent
      │            │             │
      └────────────┼─────────────┘
                   ▼
         Compare Email Drafts
                   │
                   ▼
        Select Best Email Draft
                   │
          ┌────────┴────────┐
          ▼                 ▼
 Generate Subject      Convert to HTML
          │                 │
          └────────┬────────┘
                   ▼
            Resend Email API
                   │
                   ▼
            Email Delivered
```

---

## ⚙️ Installation

Clone the repository.

```bash
git clone https://github.com/Zenitsu1Codes/Multi-Agent-Email-Writer.git

cd mail-writer
```

Create a virtual environment.

```bash
python -m venv venv
```

Activate it.

Windows

```bash
venv\Scripts\activate
```

Linux / macOS

```bash
source venv/bin/activate
```

Install dependencies.

```bash
pip install -r requirements.txt
```

---

## 🔑 Environment Variables

Create a `.env` file in the project root.

```env
GROQ_API_KEY=your_groq_api_key

OPENAI_API_KEY=your_openai_api_key

RESEND_API_KEY=your_resend_api_key

GMAIL_TO=your_email@gmail.com
```

---

## ▶️ How It Works

1. User provides a prompt requesting a sales email.
2. Three specialized AI agents generate different versions:

   * Professional
   * Humorous & Engaging
   * Concise
3. A Sales Manager agent evaluates all drafts.
4. The best draft is selected.
5. A Subject Writer agent creates an email subject.
6. An HTML Converter agent formats the email into HTML.
7. The Resend API sends the final email to the configured recipient.

---

## Example Workflow

```text
Prompt

↓

Generate 3 Email Drafts

↓

Evaluate Drafts

↓

Pick Best Version

↓

Generate Subject

↓

Convert HTML

↓

Send Email
```

---

## 📌 Example Prompt

```text
Send a cold sales email addressed to Dear CEO.
```

---

## 📧 Example Output

* Professional cold sales email
* AI-generated subject line
* HTML formatted email
* Email delivered through Resend

---

## 🎯 Learning Outcomes

This project demonstrates:

* Multi-Agent AI systems
* Agent orchestration
* Tool calling
* Parallel AI execution
* Prompt engineering
* Email automation
* API integration
* HTML email generation

---

## 🔮 Future Improvements

* Gmail API integration
* Outlook support
* Attachment support
* Lead list processing
* CRM integration
* Email tracking
* Follow-up email generation
* A/B testing of email drafts
* Web interface using Streamlit or Gradio

---

## 🤝 Contributing

Contributions are welcome.

1. Fork the repository
2. Create a new branch
3. Make your changes
4. Commit the changes
5. Open a Pull Request

---

## 👨‍💻 Author

**Harsh Asarsa**

AI • Python • Machine Learning • Agentic AI • Automation

If you found this project helpful, consider giving it a ⭐ on GitHub!
