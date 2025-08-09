# Genai
# 🤖 AI-Powered Job Recommendation System  
*Using LangChain, Google Gemini API, and Retrieval-Augmented Generation (RAG)*

---

## 📌 Project Overview

Finding the right job is challenging when job seekers are faced with huge volumes of listings and no personal guidance.  
This project is an **AI-powered job recommendation system** that takes a user's **skills**, **interests**, and **desired location** to suggest the **most relevant jobs**—along with **personalized explanations** for why each role is a great fit.  

It uses:
- **LangChain** for LLM orchestration and prompt management
- **Google Gemini API** as the Large Language Model (LLM)
- **Retrieval-Augmented Generation (RAG)** for improved accuracy via semantic search
- **Streamlit** for a simple, interactive UI

---

## 🎯 Features

- 📄 **Custom Job Input**: Load your own dataset or connect to APIs/scrapers
- 🔍 **Semantic Search (RAG)**: Retrieve the most relevant jobs before sending them to the LLM
- 💡 **AI-Powered Recommendations**: Gemini LLM suggests top matches
- 🗣 **Explanations**: Why a particular job fits your profile
- 🌐 **Web App UI**: Easy-to-use interface built in Streamlit

---

## 🛠 Tech Stack

| Component          | Technology                       |
|--------------------|-----------------------------------|
| Language           | Python                            |
| Framework          | Streamlit                         |
| LLM Orchestration  | LangChain                         |
| LLM Model          | Google Gemini                     |
| Vector Store (opt) | FAISS / Chroma                     |
| Deployment         | Local / Streamlit Cloud            |

---

## 📂 Folder Structure
---

## 🚀 Getting Started

### 1️⃣ Clone the Repository
### 2️⃣ Install Dependencies
### 3️⃣ Setup Google Gemini API Key
- Get your API key from **Google AI Studio**
- In your terminal/command prompt:
### 4️⃣ Run the App
Open the local URL shown in your terminal.

---

## 📊 How It Works

1. **User Input**: Skills, interests, and location are entered into the app.
2. **Retrieve Relevant Jobs (RAG)**:  
   - Embed job descriptions (FAISS/Chroma)
   - Find jobs semantically similar to the user's profile
3. **Generate Recommendations**:  
   - Send the top N results + user profile to Gemini via LangChain
   - Get recommended jobs with short justifications
4. **Display in UI**: Output rendered as job cards in Streamlit

---

## 💻 Sample Code Snippet
---

## 📷 Screenshots

_Add screenshots from the `/screenshots` folder here._

---

## ⚠️ Challenges & Solutions

- **Job Data Freshness**: Initially used mock dataset; future versions planned with live APIs.
- **Prompt Quality**: Iterative testing to ensure Gemini output was concise and relevant.
- **API Limits**: Managed calls with batching and careful testing.
- **Secure Key Handling**: Used environment variables to protect API keys.

---

## 📈 Future Improvements

- Live integration with job APIs/feeds
- User authentication and saved searches
- More granular filters (salary, experience level, remote/on-site)
- Feedback loop for improved AI recommendations

---

## 📚 What I Learned

- How to integrate **RAG** with an LLM (LangChain + Gemini) for more grounded recommendations  
- Techniques for **prompt engineering** to get targeted, concise answers from an LLM  
- Building and deploying an interactive **Streamlit** app quickly  
- Structuring a project for clarity and maintainability

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you’d like to change.

---

## 📜 License

This project is licensed under the MIT License - see the LICENSE file for details.
