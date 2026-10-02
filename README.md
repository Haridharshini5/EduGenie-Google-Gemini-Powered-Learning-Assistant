EduGenie - AI Educational Web Application

1. Introduction

EduGenie is an AI-based educational web application. It helps students learn easily using Artificial Intelligence.

Students can ask questions, get simple explanations, generate quizzes, summarize text, and get learning recommendations.

2. Objectives

- To help students learn easily.
- To answer students' questions using AI.
- To explain difficult topics in simple words.
- To generate quizzes for practice.
- To summarize long text.
- To recommend learning paths.

3. Technologies Used

- Python: Backend programming.
- FastAPI: Creates the backend and API.
- HTML: Creates the web page.
- CSS: Designs the web page.
- JavaScript: Handles user actions.
- Gemini API: Generates AI answers.
- Uvicorn: Runs the application.

4. Main Features

1. Question and Answer

Students can ask questions and get AI-generated answers.

Example: What is Artificial Intelligence?

2. Simple Explanation

Explains difficult topics in simple language.

Example: Explain photosynthesis in simple words.

3. Quiz Generation

Generates multiple-choice questions for students to practise.

Example: Create a quiz about the solar system.

4. Text Summarization

Summarizes long text into short and simple points.

Example: Summarize the water cycle.

5. Learning Path

Recommends learning steps based on the topic and learning level.

Example: Give me a beginner learning path for Python.

5. How It Works

1. The student opens the EduGenie website.
2. The student selects a feature.
3. The student enters a question or text.
4. The backend receives the request.
5. The AI generates the response.
6. The result is displayed on the website.

6. Project Structure

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
├── templates/
│   └── index.html
├── static/
│   └── style.css
└── tests/
    └── test_quiz.py

7. API Endpoints

Method| Endpoint| Purpose
GET| "/"| Opens the home page
POST| "/qa"| Answers questions
POST| "/explain"| Explains topics
POST| "/quiz"| Generates quizzes
POST| "/summarize"| Summarizes text
POST| "/learn/recommendations"| Recommends learning paths
GET| "/docs"| Shows API documentation

8. API Key

EduGenie uses the Google Gemini API to generate AI responses.

The API key is stored in the ".env" file.

GEMINI_API_KEY=YOUR_API_KEY
GEMINI_MODEL=gemini-2.5-flash

The API key should be kept private.

9. How to Run

Step 1: Open the project in VS Code.

Step 2: Create a virtual environment.

python -m venv .venv

Step 3: Activate the environment.

.venv\Scripts\activate

Step 4: Install the required packages.

pip install -r requirements.txt

Step 5: Add your Gemini API key to the ".env" file.

Step 6: Run the application.

uvicorn main:app --reload

Step 7: Open the website.

http://127.0.0.1:8000

10. Advantages

- Easy to use.
- Helps students understand topics.
- Provides AI-based answers.
- Makes learning interactive.
- Offers different learning features in one application.

11. Future Enhancements

- Student login.
- Save quiz results.
- Track learning progress.
- Support more languages.
- Add more quiz types.

12. Conclusion

EduGenie is an AI-powered educational web application that helps students learn easily. It provides question answering, simple explanations, quiz generation, text summarization, and learning recommendations.

The main goal of this project is to make learning simple and interactive using Artificial Intelligence.
