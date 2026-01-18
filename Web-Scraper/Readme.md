

# AI Web Scraper 🌐🤖

A powerful web scraping application built with **Streamlit**, **Selenium**, and **LangChain**. This tool allows users to scrape content from any website and use Large Language Models (LLMs) to extract specific, structured information based on natural language descriptions.

## 🚀 Features

* **Dynamic Scraping:** Uses Selenium to handle JavaScript-heavy websites.
* **DOM Cleaning:** Automatically strips scripts and styles to focus on readable text content.
* **Intelligent Parsing:** Leverages LangChain and LLMs (Ollama or Gemini) to extract only the data you need.
* **Chunked Processing:** Handles large websites by splitting content into manageable pieces for the AI.

---

## 🛠️ Tech Stack

* **Frontend:** [Streamlit](https://streamlit.io/)
* **Orchestration:** [LangChain](https://www.langchain.com/)
* **Automation:** [Selenium](https://www.selenium.dev/)
* **Parsing:** [BeautifulSoup4](https://www.crummy.com/software/BeautifulSoup/), `lxml`, and `html5lib`.
* **Environment Management:** `python-dotenv`.

---

## 📋 Prerequisites

Before running the project, ensure you have:

1. **Python 3.10 - 3.12** (Recommended for stability).
2. **Chrome Browser** installed (for Selenium).
3. An **API Key** (if using Gemini) or **Ollama** installed locally (if using Llama).

---

## ⚙️ Installation & Setup

1. **Clone the Repository:**
```bash
git clone https://github.com/your-username/web-scraper.git
cd web-scraper

```


2. **Create a Virtual Environment:**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

```


3. **Install Dependencies:**
```bash
pip install -r requirements.txt

```


---

## 🏃 How to Run

Start the Streamlit application by running:

```bash
streamlit run main.py

```

1. **Enter the URL** of the website you want to scrape.
2. **Click "Scrape Site"** to fetch and clean the DOM content.
3. **Provide a description** of what you want to extract (e.g., "Give me all product prices and names").
4. **Click "Parse Content"** to see the AI-generated results.

---

## 📁 Project Structure

* `main.py`: The Streamlit UI and application logic.
* `scrape.py`: Contains Selenium logic for fetching and cleaning web content.
* `parse.py`: Handles the LangChain logic for AI extraction.
* `requirements.txt`: List of necessary Python packages.

