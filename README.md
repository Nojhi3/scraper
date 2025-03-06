# AI-Powered Search and Aggregation Tool

## 📌 Overview
This project is an **AI-powered search and aggregation tool** that takes user input, retrieves data from multiple sources (**Google, YouTube**), processes the data using **LLM-based NLP models**, ranks the results, and presents them in an intuitive UI.

## 🚀 Features
- **FastAPI Backend**: Handles requests and fetches search results.
- **Multi-Source Data Retrieval**: Queries **Google Custom Search API** and **YouTube Data API**.
- **AI-Powered Processing**:
  - Uses **Llama API (Together AI)** to generate **search variations**.
  - Summarizes results using AI.
  - Ranks results by relevance.
- **React Frontend**: Provides an interactive UI with a search bar and structured result display.
- **Tailwind CSS Styling**: Clean, responsive, and modern design.

## 🏗️ Tech Stack
### **Backend** (FastAPI)
- **FastAPI** for high-performance API handling.
- **Together AI API** for AI-powered query processing.
- **Google Custom Search API** for Google search results.
- **YouTube Data API** for video search results.
- **Async/Await** for optimized performance.

### **Frontend** (React + TailwindCSS)
- **React (Vite)** for a fast, modular frontend.
- **Axios** for API requests.
- **Tailwind CSS** for a sleek UI.

## 📥 Installation & Setup
### **Backend Setup** (FastAPI)
1. **Clone the repository**:
   ```sh
   git clone https://github.com/yourusername/ai-search-tool.git
   cd ai-search-tool
   ```
2. **Create a virtual environment and activate it**:
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. **Install dependencies**:
   ```sh
   pip install -r requirements.txt
   ```
4. **Run FastAPI server**:
   ```sh
   uvicorn main:app --reload
   ```
5. **Verify** the API is running at:
   ```sh
   http://127.0.0.1:8000
   ```

### **Frontend Setup** (React)
1. **Navigate to frontend folder**:
   ```sh
   cd frontend
   ```
2. **Install dependencies**:
   ```sh
   npm install
   ```
3. **Run the frontend server**:
   ```sh
   npm run dev
   ```
4. **Open in Browser**:
   ```sh
   http://localhost:5173
   ```

## 🔍 How It Works
1. **User enters a search query** in the React app.
2. **Query is sent to the FastAPI backend**, where:
   - AI generates search variations.
   - Google & YouTube APIs fetch results.
   - AI ranks and summarizes results.
3. **Ranked results appear first in the UI**.
4. **Lower-ranked results are shown in a list.**

## 📸 Screenshots
![App Screenshot](https://via.placeholder.com/800x400?text=Screenshot+Coming+Soon)

## ⚙️ Environment Variables
Create a `.env` file in the backend directory and add:
```ini
YOUTUBE_API_KEY=your_youtube_api_key
TOGETHER_AI_API_KEY=your_together_ai_api_key
GOOGLE_API_KEY=your_google_api_key
GOOGLE_CSE_ID=your_google_cse_id
```

## 📚 API Reference
### **Search Endpoint**
```http
POST /search
```
#### **Request Body**
```json
{
  "query": "fastest animal"
}
```
#### **Response**
```json
{
  "query": "fastest animal",
  "results": {
    "ranked": [...],
    "google": [...],
    "youtube": [...]
  }
}
```

## 🛠️ Future Enhancements
- ✅ Add **pagination** for long search results.
- ✅ Implement **dark mode UI**.
- ✅ Improve **search query intelligence**.
- ✅ Deploy the app using **Vercel (Frontend) and Render (Backend)**.

## 📝 License
MIT License

## 🤝 Contributing
PRs are welcome! Fork the repo and create a pull request.

## ✨ Credits
Developed by [Your Name](https://github.com/yourusername) 🚀

