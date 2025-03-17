# Conversational RAG with PDF Uploads and Chat History

🚀 A **Streamlit-based Question-Answering System** Powered by **Retrieval-Augmented Generation (RAG)**

This project is a conversational question-answering system that allows users to upload **PDF documents**, ask **questions** about their content, and maintain **chat history** for context-aware responses. It leverages **RAG** and state-of-the-art **NLP models** from **Hugging Face** and **Groq**.

---

## 📌 Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Dependencies](#dependencies)

---

## 📖 Overview

This application uses **Retrieval-Augmented Generation (RAG)** to answer user questions based on the content of uploaded PDF documents. It combines:

- **Document Retrieval**: Extracts relevant information from uploaded PDFs.
- **Generative Model**: Uses **Groq's `llama-3.3-70b-versatile`** model to generate concise and accurate answers.
- **Chat History**: Maintains context across conversations for a seamless user experience.

The app is built using **Streamlit** for the frontend and integrates with **LangChain, Hugging Face, and Groq** for NLP and retrieval tasks.

---

## 🌟 Features

✅ **PDF Upload**: Upload multiple PDF files and extract their content for question-answering.  
✅ **Conversational Context**: Maintains chat history to provide context-aware responses.  
✅ **RAG Model**: Combines retrieval and generation for accurate and concise answers.  
✅ **Session Management**: Supports multiple chat sessions with unique session IDs.  
✅ **Secure API Key Input**: Securely input your **Groq API key** for model access.  

---

## 🛠 Installation

### **Prerequisites**
- **Python 3.8 or higher**
- **pip (Python package manager)**

### **Steps**

#### **1️⃣ Clone the Repository**
```sh
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

#### **2️⃣ Install Dependencies**
```sh
pip install -r requirements.txt
```

#### **3️⃣ Set Up Environment Variables**
Create a `.env` file in the root directory and add your Hugging Face token:
```ini
HF_TOKEN=your_hugging_face_token
```

#### **4️⃣ Run the Application**
```sh
streamlit run app.py
```

#### **5️⃣ Access the App**
Open your browser and navigate to **[http://localhost:8501](http://localhost:8501)**.

---

## 🚀 Usage

### **1️⃣ Enter Your Groq API Key**
On the app's homepage, enter your **Groq API key** in the provided input field.

### **2️⃣ Upload PDF Files**
Use the file uploader to **upload one or more PDF files**.

### **3️⃣ Ask Questions**
Enter your question in the text input field. The app will **retrieve relevant information** from the uploaded PDFs and generate a concise answer.

### **4️⃣ View Chat History**
The app maintains a **chat history for each session**, allowing for **context-aware conversations**.

---

## ⚙️ Configuration

### **Environment Variables**
- **`HF_TOKEN`**: Your **Hugging Face token** for accessing embeddings.
- **`GROQ_API_KEY`**: Enter your **Groq API key** in the app's interface.

### **Session Management**
Each session is identified by a **unique session_id**. You can specify a session ID or use the default (`default_session`).

### **Model Customization**
The app uses **Groq's `llama-3.3-70b-versatile`** model by default. You can modify the model in the code:
```python
llm = ChatGroq(model='llama-3.3-70b-versatile', api_key=GROQ_API_KEY)
```

---

## 📦 Dependencies

The project relies on the following **Python libraries**:

- `streamlit` → For the web interface.
- `langchain` → For RAG, document retrieval, and chat history management.
- `langchain-groq` → For integrating Groq's language models.
- `langchain-huggingface` → For Hugging Face embeddings.
- `langchain-community` → For document loaders and vector stores.
- `chroma` → For vector storage and retrieval.
- `python-dotenv` → For managing environment variables.

---

## 🏆 Acknowledgments

🙏 **Special thanks to:**

- **[Hugging Face](https://huggingface.co/)** for providing embeddings and NLP models.
- **[Groq](https://groq.com/)** for their powerful language models.
- **[LangChain](https://python.langchain.com/)** for simplifying RAG and conversational AI workflows.
- **[Streamlit](https://streamlit.io/)** for making it easy to build interactive web apps.

---

