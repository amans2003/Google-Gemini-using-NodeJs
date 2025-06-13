# Google-Gemini-using-NodeJs

# 🌟 Google Gemini API Integration with Node.js

This project demonstrates how to integrate **Google Gemini (Generative AI)** with a **Node.js Express server** to create a simple API that accepts user questions and returns AI-generated answers.

---

## 📌 Features

- Uses **Google Gemini API** for content generation.
- Exposes a REST API endpoint: `GET /api/content`.
- Accepts JSON input in the request body (via tools like **Postman**).
- Returns AI-generated responses based on the input question.

---

## 🛠 Technologies Used

- Node.js
- Express.js
- Google Gemini API (via Google Cloud Console)
- Postman (for testing)

---

## 📩 API Endpoint

**GET** `/api/content`

### 🧾 Request Body (JSON)
```json
{
  "question": "where is the redfort"
}

## Example Response
{
  "result": "The Red Fort is located in **Old Delhi, India**."
}

## API Key Setup
Visit Google Cloud Console.
Create a new project or use an existing one.
Enable the Generative AI API (Gemini API).
Generate your API key.
Store it in a .env file:

GEMINI_API_KEY=your_api_key_here

##Run Locally
git clone https://github.com/amans2003/Google-Gemini-using-NodeJs.git
cd Google-Gemini-using-NodeJs
npm install
node main.js

##Test the API
Select GET method.
URL: http://localhost:3000/api/content
Body → raw → JSON:

  {
  "question": "where is the redfort"
}

