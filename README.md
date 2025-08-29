📌 Chat App with Q/A, Edit & Delete

A simple chat-like Q&A app built with React, TailwindCSS, and Axios, connected to a backend REST API.
Users can:

Post questions

Add answers under each question

Edit or delete questions

Delete answers

🚀 Features

💬 Ask Questions – Users can add new questions (stored via API).

📝 Edit Questions – Inline editing with Save/Cancel option.

❌ Delete Questions – Remove a question permanently.

💡 Answer Questions – Reply to any question with answers.

❌ Delete Answers – Remove individual answers.

🎨 Beautiful UI – Clean inline styling with Tailwind CSS.

⚡ Real-time Updates – Updates reflect instantly in the UI.

🛠️ Tech Stack

Frontend: React, TailwindCSS

Backend: REST API (Node.js/Flask/any server exposing endpoints)

HTTP Client: Axios

📂 Project Structure
src/
│── App.jsx          # Main chat UI (Q/A, edit, delete, reply)
│── index.js         # React entry point
│── index.css        # Tailwind base styles

⚙️ API Endpoints

This app connects to the following REST endpoints (example base: https://data-sharing-apit-1.onrender.com):

Method	Endpoint	Description
GET	/home	Fetch all questions + answers
POST	/add	Add new question { comment: "text" }
PATCH	/update/:id	Update a question
DELETE	/delete/:id	Delete a question
POST	/add_answer/:questionId	Add answer to a question { answer: "text" }
DELETE	/delete_answer/:answerId	Delete answer by ID
📸 Screenshots
Questions with Actions

Users can edit or delete their questions

Answers Section

Reply box under each question

Delete button for answers

🚀 Getting Started
1. Clone Repository
git clone https://github.com/your-username/chat-app.git
cd chat-app

2. Install Dependencies
npm install

3. Setup TailwindCSS

Ensure Tailwind is configured in your project (postcss.config.js, tailwind.config.js, etc.).

Add the following to index.css:

@tailwind base;
@tailwind components;
@tailwind utilities;

4. Update API URL

Inside App.jsx, change the base URL if needed:

const API_BASE = "https://your-api-server.com";

5. Run App
npm run dev

🤝 Contributing

Fork the repo

Create a new branch (feature-new)

Commit changes

Push & create PR

📜 License

This project is open-source under the MIT License.
