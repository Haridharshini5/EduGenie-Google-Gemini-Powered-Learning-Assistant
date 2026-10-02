# EduGenie - AI Educational Web Application

## 1. Introduction

EduGenie is an AI-based educational web application. It helps students learn easily using Artificial Intelligence.

Students can ask questions, get simple explanations, generate quizzes, summarize text, and get learning recommendations.

## 2. Objectives

- To help students learn easily.
- To answer students' questions using AI.
- To explain difficult topics in simple words.
- To generate quizzes for practice.
- To summarize long text.
- To recommend learning paths.

## 3. Technologies Used

- **Python:** Used for backend development.
- **FastAPI:** Used to create the backend and API.
- **HTML:** Used to create the web page.
- **CSS:** Used to design the web page.
- **JavaScript:** Used to handle user interactions.
- **Gemini API:** Used to generate AI answers.
- **Uvicorn:** Used to run the application.
- **Jinja2:** Used to display HTML templates.

## 4. Main Features

### 4.1 Question and Answer

Students can ask questions and get AI-generated answers.

**Example:** What is Artificial Intelligence?

### 4.2 Simple Explanation

Explains difficult topics in simple language.

**Example:** Explain photosynthesis in simple words.

### 4.3 Quiz Generation

Generates multiple-choice questions for students to practise.

**Example:** Create a quiz about the solar system.

### 4.4 Text Summarization

Summarizes long text into short and simple points.

**Example:** Summarize the water cycle.

### 4.5 Learning Path

Recommends learning steps based on the topic and learning level.

**Example:** Give me a beginner learning path for Python.

## 5. How It Works

1. The student opens the EduGenie website.
2. The student selects a feature.
3. The student enters a question or text.
4. The frontend sends the request to the backend.
5. The backend processes the request.
6. The AI generates the response.
7. The response is sent back to the website.
8. The result is displayed to the student.

## 6. Project Structure

```text
EduGenie/
├── main.py
├── ai_client.py
├── qna.py
├── explanation_module.py
├── quiz_module.py
├── summary_module.py
├── learning_path.py
├── requirements.txt
├── .env
├── .gitignore
├── README.md
├── templates/
│   └── index.html
├── static/
│   └── style.css
└── tests/
    └── test_quiz.py
```

## 7. API Endpoints

| Method | Endpoint | Purpose |
|---|---|---|
| GET | / | Opens the home page |
| POST | /qa | Answers questions |
| POST | /explain | Explains topics |
| POST | /quiz | Generates quizzes |
| POST | /summarize | Summarizes text |
| POST | /learn/recommendations | Recommends learning paths |
| GET | /docs | Shows API documentation |

## 8. Gemini API Key

EduGenie uses the Google Gemini API to generate AI responses.

The API key is stored in the .env file.

Example:

```env
GEMINI_API_KEY=YOUR_API_KEY
GEMINI_MODEL=gemini-2.5-flash
```

**Note:** Keep your API key private.

## 9. How to Run the Project

### Step 1: Open the Project

Open the EduGenie folder in Visual Studio Code.

### Step 2: Create a Virtual Environment

```bash
python -m venv .venv
```

### Step 3: Activate the Environment

```bash
.venv\Scripts\activate
```

### Step 4: Install Required Packages

```bash
pip install -r requirements.txt
```

### Step 5: Add the API Key

Add your Gemini API key to the .env file.

### Step 6: Run the Application

```bash
uvicorn main:app --reload
```

### Step 7: Open the Website

http://127.0.0.1:8000

### Step 8: Open API Documentation

http://127.0.0.1:8000/docs

## 10. Advantages

- Easy to use.
- Helps students understand difficult topics.
- Provides AI-based answers.
- Makes learning interactive.
- Supports quiz practice.
- Summarizes long text.
- Provides learning recommendations.

## 11. Limitations

- Requires an internet connection for Gemini-powered features.
- Requires a valid Gemini API key.
- API usage may have limits or charges.
- AI-generated answers may sometimes be inaccurate.

## 12. Future Enhancements

- Student login and registration.
- Save quiz results.
- Track learning progress.
- Support more languages.
- Add more quiz types.
- Create a student dashboard.

## 13. Conclusion

EduGenie is an AI-powered educational web application developed using Python, FastAPI, HTML, CSS, JavaScript, and the Google Gemini API.

It helps students ask questions, understand difficult topics, practise quizzes, summarize text, and get learning recommendations.

The main goal of EduGenie is to make learning simple and interactive using Artificial Intelligence.
