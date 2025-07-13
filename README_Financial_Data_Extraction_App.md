
# 🧾 Financial Data Extraction App

A Streamlit-based application that extracts key financial metrics — **Revenue (actual & expected)** and **EPS (actual & expected)** — from textual financial news or articles using **LLM (LLaMA 3)** powered by **LangChain** and **GROQ API**.

![Streamlit](https://img.shields.io/badge/Streamlit-App-red) ![LangChain](https://img.shields.io/badge/LangChain-Integration-blue) ![LLM](https://img.shields.io/badge/LLM-Groq%2FLLaMA3-yellow)

---

## 📌 Project Overview

This application is designed to automate financial data extraction from textual news reports or earnings articles. Using an LLM (LLaMA3) served via GROQ API and integrated through LangChain, it parses raw financial text into structured JSON format output.

---

## ⚙️ Tech Stack

- **Frontend**: Streamlit
- **Backend**: Python
- **LLM API**: [Groq LLaMA3](https://groq.com/)
- **Libraries**:
  - `streamlit`
  - `langchain`
  - `langchain-groq`
  - `pyngrok`
  - `pandas`

---

## 🚀 Features

- 🧠 Extracts:
  - `revenue_actual`
  - `revenue_expected`
  - `eps_actual`
  - `eps_expected`
- 💬 Text-to-JSON financial data parsing
- ⚡ Fast and responsive due to Groq's low-latency inference
- 🌐 Publicly shareable via **ngrok**

---

## 🔧 Installation

```bash
git clone https://github.com/your-username/Financial-Data-Extraction-App.git
cd Financial-Data-Extraction-App
pip install -r requirements.txt
```

You may also manually install:

```bash
pip install streamlit pyngrok langchain_groq groq langchain-core
```

---

## ▶️ Run the App

```bash
streamlit run app.py
```

This will launch the app locally and create a public link using **ngrok**.

---

## 📤 How It Works

1. Input a financial news article into the text box.
2. The model processes the content via LangChain using a structured prompt.
3. Outputs a JSON object with extracted financial data.

---

## 🧪 Example Output

**Input Article**:
> "Apple reported earnings today. Revenue came in at $89.5B vs expected $88.9B. EPS was $1.46 beating the estimate of $1.39."

**Output JSON**:
```json
{
  "revenue_actual": "89.5B",
  "revenue_expected": "88.9B",
  "eps_actual": "1.46",
  "eps_expected": "1.39"
}
```

---

## 📁 Project Structure

```
📦 Financial-Data-Extraction-App
 ┣ 📜 Financial_Data_Extraction_App.ipynb
 ┣ 📜 app.py
 ┣ 📜 README.md
 ┗ 📜 requirements.txt
```

---

## 🛡️ Notes

- Requires **GROQ API Key** and **ngrok auth token**
- Ideal for financial analysts, traders, or data professionals looking to automate earnings parsing

---

## 🙌 Acknowledgements

- [LangChain](https://www.langchain.com/)
- [Groq](https://groq.com/)
- [Streamlit](https://streamlit.io/)
