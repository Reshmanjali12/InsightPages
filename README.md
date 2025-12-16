# InsightPages
InsightPages is an AI powered platform to upload documents (PDFs) and interact with them through conversational AI. It enables users to ask questions, generate study guides, and create flashcards from their documents using Retrieval-Augmented Generation (RAG).

---

## Features

* Upload PDF documents for analysis
* Chat with documents
* Generate Study Guides automatically
* Create Flashcards from uploaded content
* Create Quizzes
* Fast responses with LLM integration

---

## 🛠️ Tech Stack

* **Backend:** Node.js, Express.js
* **AI / NLP:** LangChain, Groq API
* **Vector Store:** FAISS
* **File Handling:** Multer, pdf-parse
* **Environment Management:** dotenv

---

## 📂 Project Structure

```
InsightPages/
├── src/
│ ├── routes/ # API routes
│ ├── services/ # Controllers & business logic
│ ├── llm/ # LLM client & vector store logic
│ ├── server.js # App entry point
├── uploads/ # Temporary uploaded files
├── .env # Environment variables
├── package.json
└── README.md
```

---

## ⚙️ Installation

1. Clone the repository

```bash
git clone https://github.com/Reshmanjali12/InsightPages.git
```

2. Navigate into the project

```bash
cd InsightPages
```

3. Install dependencies

```bash
npm init -y
npm install dotenv@^16.4.5
npm install langchain @langchain/openai @langchain/core @langchain/textsplitters
npm install langchain @langchain/groq
npm install express multer pdf-parse cors dotenv@^16.4.5
```
4. Replace package.json with this
```
{
  "name": "client",
  "private": true,
  "version": "0.0.0",
  "type": "module",
  "scripts": {
    "dev": "vite",
    "build": "vite build",
    "lint": "eslint .",
    "preview": "vite preview"
  },
  "dependencies": {
    "axios": "^1.13.2",
    "react": "^19.2.0",
    "react-dom": "^19.2.0"
  },
  "devDependencies": {
    "@eslint/js": "^9.39.1",
    "@types/react": "^19.2.5",
    "@types/react-dom": "^19.2.3",
    "@vitejs/plugin-react": "^5.1.1",
    "eslint": "^9.39.1",
    "eslint-plugin-react-hooks": "^7.0.1",
    "eslint-plugin-react-refresh": "^0.4.24",
    "globals": "^16.5.0",
    "vite": "npm:rolldown-vite@7.2.5"
  },
  "overrides": {
    "vite": "npm:rolldown-vite@7.2.5"
  }
}

```

4. Create a `.env` file

```
PORT=4000
GROQ_API_KEY=your_api_key_here
```
5. Create a client folder

```bash
npm create vite@latest client -- --template react
```
6. Navigate into the client folder

```bash
cd client
```
7. Install dependencies

```bash
npm install
npm install axios
```
8.Replace client/src/App.jsx file with the App.jsx file in git.

9.Create config.js file in client/src
```
export const BACKEND_URL = "http://localhost:4000";
```


---

## ▶️ Run the Project

```bash
npm start
```
in another terminal shell 

```bash
npm run dev
```

Server will run at:

```
http://localhost:4000
```

---

## 🧠 How It Works

1. User uploads a file or inputs text
2. Content is processed and chunked
3. Embeddings are generated and stored
4. User queries are answered using similarity search + LLM

---

## 📌 Future Improvements

* Authentication
* Better UI
* Deployment
* More AI features

---

## 🤝 Contributing

Pull requests are welcome.
For major changes, please open an issue first.

---

## 👩‍💻 Author

**Reshmanjali**
GitHub: [https://github.com/Reshmanjali12](https://github.com/Reshmanjali12)
