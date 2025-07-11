# 📰 AI-Powered News Summarizer

Effortlessly stay updated with the latest news! This project scrapes news articles from your favorite sources, uses advanced AI to summarize them, and presents everything in a beautiful, easy-to-use web interface.

---

## 🚀 Features
- **Automatic News Scraping:** Fetches the latest articles from top news sites (e.g., BBC News)
- **AI Summarization:** Uses state-of-the-art models to condense articles into bite-sized summaries
- **Clean Web UI:** Browse summaries, titles, and original links in a modern Streamlit app
- **Easy Automation:** Integrate with n8n to get news updates delivered to Discord/Telegram
- **(Optional) Topic Tagging:** Classifies articles by topic using AI
- **(Optional) Multi-Source Support:** Scrape and summarize from multiple news sites

---

## 🛠 Tech Stack
- **Python**
- **Web Scraping:** `requests`, `BeautifulSoup4`
- **AI Summarization:** Hugging Face `transformers`
- **UI:** `Streamlit`
- **Automation:** `n8n` (optional)

---

## 🧠 Skills You'll Learn
- **Web Scraping:** Inspecting web pages, extracting content with Python
- **Hugging Face Pipelines:** Using pre-trained models for summarization and classification
- **Building Web Apps:** Creating interactive UIs with Streamlit
- **Automation:** Scheduling and integrating scripts with n8n

---

## 🎓 Learning Resources
- **Web Scraping:** [Web Scraping with BeautifulSoup and Requests (FreeCodeCamp)](https://www.youtube.com/watch?v=87Gx3U0BDlo)
- **AI Summarization:** [Hugging Face Summarization Pipeline Docs](https://huggingface.co/docs/transformers/main_classes/pipelines#transformers.SummarizationPipeline)

---

## 📌 Step-by-Step Build Plan

1. **Setup**
   - Install dependencies:
     ```bash
     pip install streamlit requests beautifulsoup4 transformers torch
     ```

2. **Scraper Script**
   - Write a function to fetch a news homepage and extract article links.

3. **Article Parser**
   - Write a function to scrape the title and main text from each article link.

4. **Summarization Logic**
   - Initialize the Hugging Face summarization pipeline and summarize article text.

5. **Build UI with Streamlit**
   - Create a simple interface with a "Fetch Latest News" button.
   - Display each article's title, summary, and original link.

6. **(Optional) Automation with n8n**
   - Use n8n's Schedule node to run your script every few hours.
   - Use the Execute Command node to trigger your Python script.
   - Send new summaries to Discord/Telegram using n8n's integrations.

---

## ⚙️ Automation with n8n
- **Schedule:** Run your scraper script at regular intervals
- **Execute Command:** Trigger Python script from n8n
- **Notifications:** Post new summaries to Discord/Telegram channels

---

## 💡 Pro Tips & Optional Features
- **Topic Classification:** Use Hugging Face's zero-shot-classification pipeline to tag articles (e.g., "Technology", "Sports", "Politics")
- **Multiple Sources:** Expand to scrape from several news sites and display the source for each summary
- **Save Summaries:** Store results in a database or CSV for later reference
- **User Preferences:** Let users select topics or sources in the UI

---

## 📷 Example UI

> ![Streamlit News Summarizer Example](https://user-images.githubusercontent.com/your-image-link-here.png)

---

## 🤝 Contributing
Pull requests and suggestions are welcome! For major changes, please open an issue first to discuss what you'd like to change.

---

## 📄 License
[MIT](LICENSE)
