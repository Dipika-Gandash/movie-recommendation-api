🚀 Gemini Proxy Backend 

This is a lightweight Node.js + Express backend that works as a proxy server for Google Gemini AI.
Its main purpose is to securely handle AI requests from the frontend and return structured responses.

🔍 What this backend does

Acts as a secure proxy between the frontend and the Google Gemini API
Prevents exposing the Gemini API key in the frontend
Accepts user prompts from the frontend
Uses Gemini 2.5 Flash model to generate responses
Processes the AI response and returns clean movie recommendations

🧠 Use Case

This backend is designed for a Movie Recommendation System, where:
The user enters a search query (e.g. “funny Indian movies”)
Gemini AI generates recommendations
The backend extracts exactly movie names
Returns them as a comma-separated list converted into an array
Example response: 
{
  "movies": ["3 Idiots", "Hera Pheri", "Munna Bhai MBBS", "Chupke Chupke", "Andaz Apna Apna"]
}


🛠 Tech Stack

Node.js
Express.js
Google Gemini API (@google/genai)
dotenv – for environment variables
cors – to allow frontend access