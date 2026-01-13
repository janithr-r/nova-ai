# Nova AI - Intelligent Study Assistant 🧠🚀

**Nova AI** (formerly known as Siripala AI) is an intelligent study companion designed to help students understand lecture notes, summaries, and complex topics using the power of Google Gemini AI.

## 🌟 Features
* **AI Chat Interface:** Ask questions from your lecture notes.
* **RAG Technology:** Uses Retrieval-Augmented Generation to answer based on specific PDF content.
* **System Monitoring:** Real-time endpoints to check server health, memory usage, and system info.
* **Modern UI:** Clean and responsive interface for students.

## 🛠 Tech Stack
* **Language:** Java 17+
* **Framework:** Spring Boot 3.x
* **AI Model:** Google Gemini 1.5 Flash
* **Vector Database:** Pinecone
* **AI Integration:** LangChain4j
* **Build Tool:** Maven

## ⚙️ Configuration (Environment Variables)
⚠️ **IMPORTANT:** Never commit your API keys to GitHub. Set these variables in your IDE or Deployment platform (e.g., Render).

To run this project, you need to set the following Environment Variables:

| Variable Name | Description |
| :--- | :--- |
| `GOOGLEAI_API_KEY` | Your Google Gemini API Key |
| `PINECONE_API_KEY` | Your Pinecone Vector DB API Key |
| `PINECONE_ENV` | Pinecone Environment (e.g., us-east-1) |
| `PINECONE_INDEX_NAME` | Index name (e.g., `nova-ai`) |

## 🚀 How to Run Locally

1.  **Clone the repository**
    ```bash
    git clone (https://github.com/janithr-r/nova-ai.git)
    cd nova-ai
    ```

2.  **Open in IntelliJ IDEA**
    * Wait for Maven to download dependencies.

3.  **Set Environment Variables**
    * Go to Run Configuration -> Environment Variables and add the keys mentioned above.

4.  **Run the Application**
    * Run `AiStudyAssistantApplication.java`

5.  **Access the App**
    * Frontend: `http://localhost:8080`

## 🔌 API Endpoints (For Developers)

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/` | Home Page (Chat Interface) |
| `GET` | `/api/chat/time` | Check Server Time & Health |
| `GET` | `/api/chat/info` | View System OS & Java Version |
| `GET` | `/api/chat/memory` | Monitor Real-time RAM Usage |

---
