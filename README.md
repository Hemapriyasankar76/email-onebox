# 📧 Email Onebox - Feature-Rich Email Aggregator

## 📌 Overview
Email Onebox is a **real-time email aggregator** that synchronizes multiple IMAP email accounts, provides **AI-powered email categorization**, and offers **full-text search** with Elasticsearch. The system is similar to **Reachinbox** and includes Slack/webhook integrations for automation.

## 🚀 Features
✅ **Real-time IMAP email synchronization** (No cron jobs!)  
✅ **Elasticsearch** for **fast email search** & filtering  
✅ **AI-powered email categorization**:
   - 📩 Interested  
   - 📅 Meeting Booked  
   - ❌ Not Interested  
   - 🗑️ Spam  
   - 🚪 Out of Office  
✅ **Slack & Webhook integration** for automation  
✅ **Frontend UI** for easy email management  
✅ **AI-powered suggested replies** (Bonus Feature)  

---

## 🛠 Tech Stack
- **Backend:** FastAPI, IMAP, Elasticsearch, Python  
- **AI Model:** Machine Learning (for email categorization & suggested replies)  
- **Frontend:** React.js (Basic UI)  
- **Database:** Elasticsearch (Docker-based)  
- **Integrations:** Slack API, Webhooks  

---

## 🔧 Setup Instructions 
2️⃣ Backend Setup (FastAPI)
sh
Copy
Edit
# Create and activate a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run FastAPI server
uvicorn main:app --reload
3️⃣ Frontend Setup (React)
sh
Copy
Edit
cd frontend
npm install
npm start
4️⃣ Run Elasticsearch (Docker)
sh
Copy
Edit
docker run -d -p 9200:9200 -e "discovery.type=single-node" elasticsearch:7.10.1
