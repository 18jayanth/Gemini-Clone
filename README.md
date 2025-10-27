# 🌟 Gemini Clone — AI Chat Assistant (React + Express + Gemini API)

> A full-stack AI chat app inspired by **Google Gemini**, built using **React** for the frontend and **Express.js** for the backend.  
> This project demonstrates **secure API handling**, **AI text generation**, and a **beautiful, real-time chat interface** powered by Google's Generative AI.

---

## 🚀 Live Demo
🔗 **[gemini-clone](https://gemini-clone-vbju.vercel.app/)**

---

## 📂 Project Structure

 Gemini-Clone/
 │
 <br/>
 ├── backend/ # Express.js server
 <br/>
│ ├── server.js
<br/>
│ ├── package.json
<br/>
│ ├── .env # Store Gemini API key here
<br/>
│ └── .gitignore
│
<br/>
├── frontend/ # React.js client
<br/>
│ ├── src/
<br/>
│ ├── public/
<br/>
│ ├── package.json
<br/>
│ └── .gitignore
<br/>
│

└── README.md


---

## ✨ Features

- 🤖 **AI Chat with Gemini API** – Real-time responses using Google’s Generative AI.
- 🔒 **Secure Backend** – API key is hidden using environment variables (`.env` file).
- ⚡ **Fast Response Handling** – Backend proxy ensures smooth and secure communication.
- 💬 **Modern UI** – React frontend styled to resemble Gemini’s sleek design.
- 🧠 **Custom Safety Filters** – Uses `HarmCategory` and `HarmBlockThreshold` to prevent unsafe responses.

---

## 🧰 Tech Stack

| Layer | Technologies Used |
|-------|--------------------|
| **Frontend** | React.js, Fetch API, CSS |
| **Backend** | Node.js, Express.js |
| **AI Model** | Google Generative AI (Gemini 1.5 or 2.0) |
| **Environment** | dotenv |
| **Security** | CORS, Environment Variables |
| **Deployment** | Vercel (frontend), Render/Railway (backend) |

---

## ⚙️ Installation & Setup
```bash
Follow these steps to set up locally 👇

### 1️⃣ Clone the repository
git clone https://github.com/18jayanth/Gemini-Clone.git
cd Gemini-Clone


Backend Setup
cd backend
npm install



Create a .env file inside backend/:

GEMINI_API_KEY=your_api_key_here
PORT=5000


Then run:

npm start


The backend runs on http://localhost:5000

3️⃣ Frontend Setup
cd ../frontend
npm install
npm start


The frontend runs on http://localhost:5500

4️⃣ Connect Frontend ↔ Backend

In your frontend’s API call (e.g., generateImage.jsx or chat.js), set:

fetch("http://localhost:5000/api/chat", {
  method: "POST",
  headers: { "Content-Type": "application/json" },
  body: JSON.stringify({ prompt }),
});
```
🧠 How It Works

User enters a prompt in the React frontend.

The frontend sends this prompt to the backend (/api/chat endpoint).

The Express backend securely forwards it to Gemini API using your hidden API key.

The Gemini model processes and returns the generated text.

The backend responds with the AI’s output, which is then displayed beautifully in the UI.

🖼️ Screenshots
Feature	Screenshot
💬 Chat Interface  

🛠️ Environment Setup Notes
File	Purpose
.env	Stores API keys like GEMINI_API_KEY (⚠️ do not upload to GitHub)
.gitignore	Must include .env to prevent key leaks
package.json	Dependencies for both frontend & backend
server.js	Main backend entry file
💡 Future Improvements

🧑‍💻 Add chat history with MongoDB

🎤 Integrate voice input/output

🌙 Dark mode toggle

🧠 Multi-model switch (Gemini, GPT, Claude)

📱 Mobile-responsive UI enhancements



🙌 Acknowledgements

Google Generative AI

React

Express.js

Inspiration from Google Gemini’s interface

👨‍💻 Author

Jayanth
📍 Machine Learning & Full Stack Enthusiast
🔗 [Github](https://github.com/18jayanth)
