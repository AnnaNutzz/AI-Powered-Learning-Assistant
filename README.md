# AI-Powered Learning Assistant 📚🤖

A Flask web app that helps students learn based on their preferred learning style. The system offers automatic note summarization from uploaded files (PDF, PPTX, TXT), stores personalized content in Notion, and sends progress updates via SMS using Twilio.

## 🔧 Features

- 🧠 Personalized learning style detection (quiz-based)
- 📤 File upload (PDF, PPTX, TXT)
- ✨ AI-generated summaries via Ollama + Hugging Face Transformers
- 🗒️ Notes auto-added to Notion
- 📲 SMS notifications to parents using Twilio
- 📊 Dashboard with learning suggestions

## 🛠️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/AnnaNutzz/ai-learning-assistant.git
cd ai-learning-assistant
```

### 2. Create a virtual environment

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Create a `.env` file

```env
FLASK_SECRET_KEY=your_flask_secret_key
NOTION_SECRET=your_notion_integration_token
NOTION_DATABASE_ID=your_notion_db_id
TWILIO_PHONE_NUMBER=+1234567890
TWILIO_SID=your_twilio_sid
TWILIO_AUTH_TOKEN=your_twilio_auth_token
```

## ▶️ Run the app

```bash
python your_main_file.py
```

Visit http://localhost:5000

## 📝 Usage Flow

1. Register or log in.
2. Take the learning style quiz.
3. Upload study material.
4. Get auto-generated summaries.
5. Summaries saved in:
   - Local database
   - Notion workspace
6. Parent gets SMS updates after revision.

## 📁 Project Structure

```
/uploads            - Uploaded files
/templates          - HTML templates
.env                - Secrets and config
app.py              - Main Flask app
```

## ✅ Dependencies

- Flask
- SQLite
- pdfplumber
- python-pptx
- HuggingFace Transformers
- Twilio
- Notion SDK      #doesn't work
- Ollama
- python-dotenv
