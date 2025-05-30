# 🤖 AI Empathy Gemini Project

A web-based application demonstrating AI-generated empathetic responses using Google's **Gemini API** via **Google AI Studio**. The goal of this project is to showcase how artificial intelligence can simulate emotional intelligence and respond with compassion and understanding to user inputs.

---

## 🚀 Features

- 🌟 Uses **Gemini API** to generate human-like empathetic responses  
- 🔄 Interactive frontend built with **Streamlit**  
- 🔧 Backend powered by **FastAPI**  
- 💬 RESTful API endpoint for generating responses  

---

## 🛠️ Setup Instructions

Follow these steps to set up and run the project locally:

### 1. Clone the repository

```bash
git clone https://github.com/your-username/ai-empathy-gemini.git
cd ai-empathy-gemini
```

### 2. Create and activate a virtual environment

#### Linux/macOS:
```bash
python3 -m venv .venv
source .venv/bin/activate
```

#### Windows:
```bash
python -m venv .venv
.venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Set up your Gemini API key

Create or edit the file `backend/config.py`:

```python
# backend/config.py

GEMINI_API_KEY = "your_api_key_here"
```

> 💡 Replace `"your_api_key_here"` with your actual Gemini API key obtained from [Google AI Studio](https://makersuite.google.com/app).

### 5. Run the backend server

```bash
uvicorn backend.main:app --reload
```

### 6. Launch the frontend app

```bash
streamlit run frontend/app.py
```

---

## 📡 Backend API Endpoint

- **POST** `/chat/generate_response/`

  **Description**: Takes user input and returns an AI-generated empathetic response.

  **Payload Example**:

  ```json
  {
    "message": "I'm feeling really overwhelmed with work lately."
  }
  ```

  **Response Example**:

  ```json
  {
    "response": "I'm sorry you're feeling overwhelmed. Remember to take breaks and prioritize your well-being. You're doing your best, and that's enough."
  }
  ```

---

## 📋 Usage Guide

1. Start both backend and frontend services.  
2. Open the Streamlit UI in your browser (typically at `http://localhost:8501`).  
3. Type a message expressing an emotional state or concern.  
4. View the empathetic AI-generated response in real-time.  

---

## 🤝 Contributing

Feel free to fork this project, raise issues, and contribute improvements! Whether it's adding features, fixing bugs, or improving UI, contributions are welcome.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🙏 Acknowledgments

- [Google AI Studio](https://makersuite.google.com/)
- [FastAPI](https://fastapi.tiangolo.com/)
- [Streamlit](https://streamlit.io/)
