🤖 AI Customer Support Bot

![image alt](https://github.com/rajatrajat0210/AI-CustomerSupportBot/blob/main/AI-Chatbot-Frontend.jpg?raw=true)

✨ AGENTS IN LANGFLOW MODEL

![image alt](https://github.com/rajatrajat0210/AI-CustomerSupportBot/blob/main/agents_langflow.jpg?raw=true)

✨ FULL FLOW MODEL FOR LANGFLOW 

![image alt](https://github.com/rajatrajat0210/AI-CustomerSupportBot/blob/main/langflow.jpg?raw=true)

✨ PDF TO VECTOR DATA FOR EASY SEARCH

![image alt](https://github.com/rajatrajat0210/AI-CustomerSupportBot/blob/main/pdftovector.jpg?raw=true)

   

🚀 Overview

Welcome to the AI Customer Support Bot! This AI-powered chatbot is designed to enhance customer experience by providing instant responses to FAQs, order lookups, and product-related inquiries. Built using Groq APIs, Streamlit, and Langflow, it seamlessly integrates with Astra DB to fetch and store structured data. Additionally, it supports PDF parsing for easy access to business-related data.

✨ Features

✅ AI-driven responses powered by Groq APIs - (llama 3-70b versatile)
✅ Interactive Streamlit UI for a seamless user experience (Custom and easy to build Front-end)
✅ Langflow-powered agent-based system for efficient query handling (Low Code Based Tool for implementing AI and DB flows to build Agents)
✅ Main Manager Agent that routes queries to:
     📌 FAQ Agent (answers business & product-related questions)
     📦 Order Lookup Agent (retrieves order details from Astra DB)
     📦 Product Lookup Agent (retrives product details from Astra DB)
     
✅ Astra DB integration for storing & retrieving orders, products, and FAQs✅ PDF parsing support to extract and utilize business data efficiently

🏗️ Architecture

graph TD;
  User -->|Queries| Streamlit UI -->|Routes to| Main_Manager_Agent;
  Main_Manager_Agent -->|Handles FAQs| FAQ_Agent;
  Main_Manager_Agent -->|Looks up orders| Order_Lookup_Agent;
  Main_Manager_Agent -->|Looks up products| Product_Lookup_Agent;
  Order_Lookup_Agent -->|Fetches Data| Astra_DB;
  Product_Lookup_Agent -->|Fetches Data| Astra_DB;


🔧 Installation

📌 Prerequisites

Ensure you have the following installed:

🐍 Python 3.8+

🌐 Streamlit

⚡ Langflow

🛢️ Astra DB account

🔑 Groq API Key

📥 Clone the Repository

git clone https://github.com/your-username/ai-support-bot.git
cd ai-support-bot

📦 Install Dependencies
```bash
pip install -r requirements.txt
```
🛠️ Set Up Environment Variables

Create a .env file and add your credentials:

ASTRA_DB_ID=<your_astra_db_id>
ASTRA_DB_REGION=<your_astra_db_region>
ASTRA_DB_KEYSPACE=<your_keyspace>
ASTRA_DB_APPLICATION_TOKEN=<your_application_token>
GROQ_API_KEY=<your_groq_api_key>

▶️ Run the Bot
```bash
streamlit run app.py
```
🎯 Usage

Open the Streamlit UI in your browser.

Ask questions about orders, products, or general business inquiries.

Bot fetches relevant information from Astra DB or parsed PDFs.

AI-powered responses are delivered in real-time! 🚀

🌍 Deployment

For deploying on Streamlit Cloud or other cloud providers, ensure that your API keys and secrets are properly configured.

🤝 Contribution

Contributions are welcome! 🚀

Fork the repo

Create a feature branch

Submit a pull request
