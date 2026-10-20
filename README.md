ScamGuard AI

Project Overview
ScamGuard AI is a scam detection application that uses Large Language Models (LLMs) to analyze text messages and identify potentially fraudulent or manipulative communications.
The project addresses the problem of digital scams that use urgency, fear, impersonation, fake rewards, and other psychological tactics to deceive people. It uses the Google Gemini API to analyze messages and classify them as Scam, Not Scam, or Uncertain.
The goal is to make scam detection more context-aware and provide explanations that help users understand why a message may be suspicious.

Key Features
Classifies messages as Scam, Not Scam, or Uncertain.
Identifies the possible type of scam, including phishing, OTP fraud, fake rewards, account suspension threats, and loan scams.
Analyzes manipulative intent, such as urgency, fear, and impersonation.
Provides explanations for classification results.
Uses prompt engineering techniques for message analysis.
Follows a modular structure so individual components can be maintained and extended.
Provides a user interface through Streamlit.

Technology Stack

Python 3.12+
Google Gemini API
Streamlit
Pandas
Python-dotenv
Pydantic

Project Structure
The project contains the main application, Streamlit interface, configuration, utility functions, and pipeline components.

Setup Instructions
1. Clone the repository
git clone <repository-url>
cd ScamGuard-AI

2. Create a virtual environment
For macOS:
python3.12 -m venv .venv
source .venv/bin/activate

For Windows:
py -3.12 -m venv .venv
.venv\Scripts\activate

3. Install dependencies
python -m pip install -r requirements.txt

4. Configure the API key
Create a .env file in the project root and add your Google Gemini API key:
GEMINI_API_KEY=your_api_key_here
Keep the .env file private and do not upload API keys or other sensitive information to GitHub.

5. Run the application
Run the main Python application:
python main.py

Start the Streamlit interface:
streamlit run app.py

Testing and Evaluation
The project use case includes a scam detection dataset containing message text and corresponding labels. The dataset can be used to test the application's ability to identify scam and legitimate messages.
Testing should include phishing attempts, OTP requests, fake rewards, account suspension messages, loan offers, legitimate notifications, and ambiguous messages.
The results can be evaluated based on classification accuracy, false positives, false negatives, and the quality of the explanations.


Demo screen


<img width="794" height="589" alt="Screenshot 2026-10-20 at 10 52 47 PM" src="https://github.com/user-attachments/assets/0cf54a72-4a9d-40a6-80bd-406d6e8cc528" />
