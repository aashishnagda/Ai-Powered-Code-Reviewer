# Ai-Powered-Code-Reviewer

An AI-powered code review application built using the MERN stack. The application allows users to write JavaScript code in an integrated code editor, send it to the backend, and receive AI-generated code review suggestions.

## ✨ Features

- 📝 Built-in JavaScript code editor
- 🤖 AI-powered code review
- 💡 Suggestions for code quality and best practices
- 🎨 Syntax highlighting for both input and reviewed code
- ⚡ Fast React + Vite frontend
- 🔗 REST API integration between frontend and backend

---

## 🛠️ Tech Stack

### Frontend

- React
- Vite
- Axios
- React Simple Code Editor
- PrismJS
- React Markdown
- Highlight.js

### Backend

- Node.js
- Express.js
- Google Gemini API
- dotenv
- CORS

---

## 📂 Project Structure

```
Ai-Powered-Code-Reviewer
│
├── BackEnd
│   ├── src
│   │   ├── controllers
│   │   ├── routes
│   │   └── services
│   ├── server.js
│   ├── package.json
│   └── .env
│
├── Frontend
│   ├── src
│   ├── public
│   ├── package.json
│   └── vite.config.js
│
└── README.md
```

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/aashishnagda/Ai-Powered-Code-Reviewer.git
```

```
cd Ai-Powered-Code-Reviewer
```

---

### 2. Install Backend Dependencies

```bash
cd BackEnd
npm install
```

---

### 3. Install Frontend Dependencies

```bash
cd ../Frontend
npm install
```

---

## 🔑 Environment Variables

Create a `.env` file inside the **BackEnd** folder.

```env
GOOGLE_GEMINI_KEY=YOUR_API_KEY
```

> **Note:** Generate your own Gemini API key from Google AI Studio.

---

## ▶️ Run the Backend

```bash
cd BackEnd
node server.js
```

---

## ▶️ Run the Frontend

```bash
cd Frontend
npm run dev
```

---

## 🚀 How It Works

1. Write JavaScript code in the editor.
2. Click the **Review** button.
3. The frontend sends the code to the Express backend.
4. The backend forwards the request to the Gemini API.
5. The AI analyzes the code and returns suggestions.
6. The reviewed output is displayed with Markdown formatting and syntax highlighting.

---

## 📌 API Endpoint

### Review Code

```
POST /ai/get-review
```

### Request Body

```json
{
  "code": "function sum(){ return 1+1; }"
}
```

---

## 📸 Screenshots

You can add screenshots of:

- Home Page
- Code Editor
- AI Review Output

---

## 🔮 Future Improvements

- Support multiple programming languages
- Authentication
- Review history
- Export review as PDF
- Theme switch (Dark / Light)
- AI provider abstraction for switching between Gemini, OpenRouter, OpenAI, etc.

---

## 👨‍💻 Author

**Aashish Nagda**

GitHub: https://github.com/aashishnagda

---

## ⭐ If you found this project useful, consider giving it a star.