SnackSnap 

SnackSnap is an AI-powered food tracking and alert assistant built with **Streamlit**. It uses the **Google Gemini 3.8-Flash** model to analyze food items or images and instantly delivers summaries or automated text alerts directly to users using the **Twilio API**.

## 🚀 Features
* **AI Food Analysis:** Leverages Gemini 3.8-Flash to provide nutritional insights or quick text summaries of food.
* **SMS Notifications:** Integrates Twilio Client to send instant text alerts to your mobile device.
* **Streamlit UI:** A clean, easy-to-use, and responsive local web dashboard.

## 🛠️ Tech Stack
* **Frontend/Dashboard:** Streamlit
* **AI Model:** Google Gemini 3.8-Flash (Google AI Studio)
* **Communications:** Twilio Python SDK
* **Language:** Python 3.x

## 💻 Installation & Setup

Follow these steps to run the project locally on your machine:

### 1. Clone the Repository
```bash
git clone https://github.com
cd SnackSnap
```

### 2. Set Up a Virtual Environment
```powershell
# Create venv
python -m venv venv

# Activate venv (Windows PowerShell)
.\venv\Scripts\Activate.ps1
```

### 3. Install Dependencies
```bash
pip install streamlit twilio google-generativeai
```

### 4. Configure Your Secrets
Create a `.streamlit/secrets.toml` file in the project root directory and add your private API keys:
```toml
GEMINI_API_KEY = "YOUR_GEMINI_API_KEY"
# Add your Twilio credentials here if needed
# TWILIO_ACCOUNT_SID = "YOUR_SID"
# TWILIO_AUTH_TOKEN = "YOUR_TOKEN"
```

### 5. Run the Application
```bash
streamlit run app.py
```

## 🛡️ Security Note
Your local `.streamlit/secrets.toml` configuration file contains private API keys and is safely omitted from version control via `.gitignore`.
