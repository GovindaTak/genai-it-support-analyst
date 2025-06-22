# genai-it-support-analyst
A GenAI-powered IT Support Analyst assistant that classifies and responds to multilingual IT support tickets using OpenAI GPT-4o and LangChain. Converts raw customer queries into structured JSON outputs with categorization, translation, and personalized response.


````markdown
# 🤖 GenAI IT Support Analyst

A hands-on LangChain & OpenAI project that simulates an intelligent **IT support analyst agent** capable of reading multilingual IT tickets, detecting language, translating the message, classifying the issue, and generating responses in both the original and English language.

---

## 🎯 Project Objective

To build an AI-powered agent that:
- Accepts multilingual IT tickets
- Translates them to English
- Classifies the category of issue (Login Issue, Network, Printer, etc.)
- Provides a structured JSON response
- Responds back in original and English languages

---

## ⚙️ Technologies & Tools

- 🧠 OpenAI GPT-4o (via `langchain_openai`)
- 🧱 LangChain core + community
- 🐍 Python 3.11+
- 🧾 Pydantic for structured validation
- 📊 Pandas for result tabulation

---

## 🛠️ Features

- 🌍 **Language Detection**: Supports Portuguese, Russian, Japanese, Turkish, Italian, and more.
- 🧠 **Prompt-Oriented Classification**: Zero-shot task classification using LLMs.
- 📤 **Response Generation**: Localized and translated customer responses.
- 🧾 **Structured JSON Output**: Returns valid JSON with detailed fields.
- 📦 **Batch Processing**: Processes ticket queues at once using `.map()` in LangChain.

---

## 🧪 Sample Output (JSON)

```json
{
  "orig_msg": "Ho problemi a stampare i documenti da remoto...",
  "orig_lang": "Italian",
  "category": ["Printing", "Remote Access"],
  "trans_msg": "I have problems printing documents remotely...",
  "response": "Per risolvere il problema, ti consiglio di...",
  "trans_response": "To resolve the issue, I recommend..."
}
````

---

## 🧠 Skills Learned

✅ LangChain prompt pipeline with structured output
✅ OpenAI model usage for classification and translation
✅ Pydantic data modeling and JSON parsing
✅ Internationalization and localization handling with LLMs
✅ LangChain `.map()` for batch inference
✅ Interfacing multilingual input with robust fallback logic
✅ End-to-end automation for support systems


## 🚀 How to Run

```bash
# 1. Clone the repo
git clone https://github.com/GovindaTak/genai-it-support-analyst.git
cd genai-it-support-analyst

# 2. Install dependencies


# 3. Add your OpenAI key securely
export OPENAI_API_KEY='your-api-key'

# 4. Run the notebook or script
jupyter notebook it_support_analyst.ipynb
```

---

## 📌 Future Enhancements

* ✅ Add Streamlit UI for interactive demo
* ✅ Connect with real-time email parser or ITSM systems
* ✅ Use Vector Store + RAG for KB-based responses
* ✅ Extend support for image-based tickets (OCR)

---

## 🙏 Special Thanks

To **OpenAI**, **LangChain**, and all the communities sharing GenAI knowledge.
Built with ❤️ by **Govinda Tak** as part of learning and development.
