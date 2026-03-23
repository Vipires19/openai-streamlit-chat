# 🤖 PirecoBot - Streamlit Chatbot with OpenAI

A simple conversational AI chatbot built with **Streamlit** and **OpenAI API**, featuring real-time streaming responses and local conversation persistence.

This project demonstrates how to build an interactive chat interface with session management and saved conversations — ideal as a foundation for more advanced AI applications.

---

## 🚀 Features

- 💬 Chat interface using Streamlit
- ⚡ Real-time streaming responses from OpenAI
- 🧠 Context-aware conversations
- 💾 Local conversation persistence using pickle
- 📂 Sidebar with conversation history
- 🔄 Ability to switch between past conversations
- 🧹 Automatic conversation naming based on user input

---

## 🛠️ Tech Stack

- **Python**
- **Streamlit**
- **OpenAI API (gpt-3.5-turbo)**
- **Pickle (local storage)**
- **dotenv**

---

## 📁 Project Structure


.
├── app.py
├── conversas_salvas/
├── .env
└── README.md


---

## ⚙️ Installation

1. Clone the repository:

```bash
git clone https://github.com/your-username/pirecobot.git
cd pirecobot
Create a virtual environment:
python -m venv venv
source venv/bin/activate  # Linux / Mac
venv\Scripts\activate     # Windows
Install dependencies:
pip install -r requirements.txt
Set your OpenAI API key:

Create a .env file or use Streamlit secrets:

OPENAI_API_KEY=your_api_key_here
▶️ Running the App
streamlit run app.py
🧠 How It Works
The app uses Streamlit session state to manage chat history.
Messages are sent to the OpenAI API using streaming (stream=True) for real-time responses.
Conversations are saved locally using pickle, allowing users to revisit past chats.
Each conversation is automatically named based on the first user message.
📌 Key Implementation Details
Streaming responses for better UX
File-based persistence layer (no database required)
Dynamic conversation loading
Sanitized file naming using regex + unidecode
⚠️ Limitations
Uses local storage (not scalable for production)
No authentication or user management
Relies on pickle (not ideal for secure environments)
🔮 Future Improvements
Replace pickle with a database (MongoDB / PostgreSQL)
Add user authentication
Deploy as a SaaS application
Improve UI/UX
Add conversation search
Integrate embeddings for semantic memory
📷 Demo

You can add screenshots or a GIF here

📄 License

This project is open-source and available under the MIT License.

👨‍💻 Author

Developed by Vinícius Pires
