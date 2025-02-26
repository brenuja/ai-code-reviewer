# AI-Powered Code Reviewer

## 🚀 Overview
This project is an **AI-powered code reviewer** that provides detailed feedback on code quality, best practices, efficiency, security, scalability, and maintainability. It leverages **Google Gemini API** to generate AI-driven code reviews.

## 🛠 Tech Stack
- **Backend:** Node.js, Express.js
- **AI Model:** Google Gemini API
- **Environment Variables:** dotenv
- **Security & CORS:** cors

## 📂 Project Structure
```
Backend/
├── src/
│   ├── app.js          # Main Express app configuration
│   ├── routes/
│   │   ├── ai.routes.js    # Routes for AI code review
│   ├── controllers/
│   │   ├── ai.controller.js  # Handles requests & responses
│   ├── services/
│   │   ├── ai.service.js  # Interacts with Google Gemini API
├── server.js       # Server entry point
├── .env            # Environment variables (ignored in Git)
```

## 🚀 Getting Started
### 1️⃣ Clone the Repository
```sh
git clone https://github.com/your-username/your-repo-name.git
cd ai-code-reviewer
```

### 2️⃣ Install Dependencies
```sh
npm install
```

### 3️⃣ Setup Environment Variables
Create a `.env` file in the root directory and add:
```
GOOGLE_GEMINI_KEY=your_google_gemini_api_key
PORT=3000
```

### 4️⃣ Start the Server
```sh
npm start
```
> Server will be running on `http://localhost:3000`

## 📌 API Endpoints
### 🔹 Test Server
**GET /** → Returns a simple welcome message.
```sh
curl http://localhost:3000/
```

### 🔹 Get AI Code Review
**POST /ai/get-review** → Sends code to AI for review and receives feedback.

#### Request Body (JSON):
```json
{
    "code": "function add(a, b) { return a + b; }"
}
```

#### Response:
```json
{
    "review": "✔ Your function follows best practices, but consider adding input validation."
}
```

## 🛠 Features
✅ AI-driven code analysis  
✅ Best practice recommendations  
✅ Security and performance suggestions  
✅ Scalability and maintainability insights  
✅ Constructive and professional feedback  

## 🤝 Contributing
Feel free to open an issue or submit a pull request if you want to improve the project!

## 📜 License
This project is **MIT Licensed**.

---
**🚀 Happy Coding!**

