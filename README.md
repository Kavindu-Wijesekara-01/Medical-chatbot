# 🏥 Medical Chatbot

A Medical Chatbot powered by LLMs, Langchain, Pinecone, and Flask.

---

## 🛠️ Tech Stack

- **LLM** - Groq (Llama 3)
- **Embeddings** - HuggingFace (`all-MiniLM-L6-v2`)
- **Vector Store** - Pinecone
- **Framework** - Langchain
- **Backend** - Flask
- **Language** - Python 3.10

---

## ⚙️ Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/Kavindu-Wijesekara-01/Medical-chatbot.git
cd Medical-chatbot
```

### 2. Create a Conda Environment
```bash
conda create -n medibot python=3.10 -y
conda activate medibot
```

### 3. Install Requirements
```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables

Create a `.env` file in the root directory:
```
PINECONE_API_KEY="your_pinecone_api_key"
GROQ_API_KEY="your_groq_api_key"
```

### 5. Store the Medical Data in Pinecone
```bash
python store_index.py
```

### 6. Run the Application
```bash
python app.py
```

Open browser: `http://localhost:8080`

---

## 📁 Project Structure
```
Medical-chatbot/
├── data/
│   └── Medical_book.pdf
├── src/
│   ├── helper.py
│   └── prompt.py
├── templates/
│   └── chat.html
├── app.py
├── store_index.py
├── requirements.txt
├── .env
└── README.md
```

---

## 🔑 Required API Keys

| Service  | Purpose         | Free Tier |
|----------|-----------------|-----------|
| Pinecone | Vector Database | ✅ Yes    |
| Groq     | LLM (Llama 3)   | ✅ Yes    |

---

## 📄 License

Apache 2.0 License