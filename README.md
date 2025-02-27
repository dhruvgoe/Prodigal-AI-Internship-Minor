# DhruvSummariser - Multi Agent Author

## 📄 Project Overview
This project is a **Multi-Agent Author System** developed for the **Prodigal AI Internship**. The system is designed to:
- **Scrape** a target website and store the data in a CSV file.
- **Summarize** the extracted content using the **Google Gemini API**.
- **Send the generated summaries** to Telegram on **phone or desktop** using a **Telegram Bot**.

## 🚀 Features
- **CSV Upload**: Upload a CSV file containing articles.
- **AI-Powered Summarization**: Uses **Google Gemini API** to generate concise summaries.
- **Telegram Integration**: Automatically sends summaries to a **Telegram chat**.
- **Streamlit UI**: Simple and interactive web-based interface.

## 🛠️ Tech Stack
- **Python** (Main Programming Language)
- **Streamlit** (Frontend UI for user interaction)
- **Google Gemini API** (For AI-powered text summarization)
- **Telegram Bot API** (For sending summaries to Telegram)
- **Pandas** (For handling CSV data)
- **Asyncio & Nest Asyncio** (For asynchronous messaging)

## 📂 Project Structure
```
📦 DhruvSummariser
├── .env                   # Environment variables (API keys & Bot credentials)
├── app.py                 # Main Streamlit application
├── requirements.txt       # Python dependencies
└── README.md              # Project Documentation
```

## 🔧 Installation & Setup
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/DhruvSummariser.git
cd DhruvSummariser
```

### 2️⃣ Create a Virtual Environment (Optional but Recommended)
```bash
python -m venv venv
source venv/bin/activate  # On macOS/Linux
venv\Scripts\activate     # On Windows
```

### 3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 4️⃣ Set Up API Keys & Bot Credentials
- Create a `.env` file in the project root and add:
```
TOKEN=your_telegram_bot_token
CHAT_ID=your_telegram_chat_id
API_KEY=your_google_gemini_api_key
```

## ▶️ Running the Application
Run the Streamlit app using:
```bash
streamlit run app.py
```

## 📤 Usage
1. **Upload a CSV file** containing `Article Name` and `Article Content` columns.
2. **Click 'Generate'** to generate AI-powered summaries for the first two articles.
3. **View the summaries** in the text area.
4. **Click 'Send Summaries to Telegram'** to send the summaries to your Telegram chat.

## 📝 Example CSV Format
| Article Name | Article Content |
|-------------|----------------|
| AI in Healthcare | AI is revolutionizing the healthcare industry by... |
| Future of Quantum Computing | Quantum computing is set to change the world by... |

## 🛑 Troubleshooting
- Ensure the `.env` file contains the correct API keys.
- If the **Telegram bot doesn't send messages**, check if the bot has permission to message the user.
- If the **summarization fails**, ensure the Google Gemini API key is valid.

## 📌 Future Enhancements
- Expand support to summarize **more than 2 articles** at a time.
- Implement **custom summarization length** options.
- Enable **multi-language summarization** support.

## 📜 License
This project is licensed under the **MIT License**.

## 📬 Contact
For any issues or queries, feel free to reach out via GitHub Issues!
