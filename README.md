# 🧠 AI AutoCodeReview

 Developed an **AI AutoCodeReview** tool using Node.js, Express, React.js, and Google Generative AI. Enabled
 intelligent feedback generation via POST requests, with syntax highlighting (PrismJS) and Markdown rendering
 for clean code display.

---

## 🚀 Features

- 🤖 **AI-Powered Code Review**  
  Instantly analyzes code and provides intelligent suggestions using Google Generative AI.

- ⚡ **Real-Time Feedback**  
  Submit code and get instant AI-generated reviews via POST requests.

- 🎨 **Syntax Highlighting**  
  Code is displayed with clean, colorful formatting using **PrismJS**.

- 📝 **Markdown Rendering**  
  Feedback is shown in a clean, structured format using **React Markdown**.

- 🔧 **Modular Full-Stack Architecture**  
  Built with a clean separation between frontend and backend for scalability.

---

## 🧰 Tech Stack

### 🔹 Frontend
- React.js (Vite) – Fast, modern frontend setup
- PrismJS – Beautiful syntax highlighting
- React Markdown – Render formatted AI feedback
- Axios – For HTTP requests

### 🔹 Backend
- Node.js & Express.js – Efficient REST API backend
- Google Generative AI (PaLM/Gemini) – Natural language processing & code understanding

---

## 📸 Screenshots

### 🖥️ 1. Home Interface – Code Input and Review Layout

The user lands on a modern interface split into two main sections:
- **Left Panel** – Code input area with syntax highlighting  
- **Right Panel** – Output area showing AI-reviewed feedback, issues, suggestions, and improvements.

![Code Review UI](FrontEnd/public/home.png)


---

### ✏️ 2. Code Input Section
User enters or pastes their code in a text area with syntax highlighting.

![Code Input](FrontEnd/public/input.png)

---

### 🖱️ 3. Click "Review" Button
User clicks the "Review" button to submit code for AI evaluation.

![Review Button](FrontEnd/public/review.png)

---

### 📤 4. AI-Generated Feedback Output
AI responds with clean, Markdown-formatted suggestions and improvements.

![AI Output](FrontEnd/public/output.png)

---

## ✍️ Input & Output Details

### ✅ Input
Users can submit code snippets in any language through the input field. The code is sent to the backend via a POST request.

### Example Code:

```javascript
function sum() {
  return a + 3;
}

### ✅ Output
❌ Bad Code:

function sum() {
  return a + 3;
}
🔍 Issues:

❌ a is not defined within the scope of the function, likely causing an error or unexpected behavior.
❌ The function doesn't accept any arguments, making it inflexible and only useful for a specific, predefined a.
✅ Recommended Fix:

function sum(a) {
  return a + 3;
}
💡 Improvements:

✔ The function now accepts a as an argument, making it reusable and flexible.
✔ It clearly defines the scope of a, preventing any undefined variable errors.
