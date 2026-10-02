EduGenie Project – Overall Overview

1. Project Introduction

Project Name: EduGenie
Project Type: AI-Based Educational Web Application

EduGenie is an AI-powered educational web application designed to make learning easier and more interactive for students. It uses Artificial Intelligence to answer questions, explain difficult topics, generate quizzes, summarize text, and recommend learning paths.

The main aim of EduGenie is to help students understand their lessons and improve their learning experience.

2. Project Objectives

- To provide AI-based answers to students' questions.
- To explain difficult topics in simple language.
- To generate quizzes for practice.
- To summarize long educational content.
- To recommend personalized learning paths.
- To make learning easier and more interactive.

3. Technologies Used

1. Python: Main programming language used for backend development.
2. FastAPI: Framework used to create the backend and API endpoints.
3. HTML: Used to create the structure of the web page.
4. CSS: Used to design and style the web page.
5. JavaScript: Used to handle user interactions and communicate with the backend.
6. Google Gemini API: Used to generate AI-based answers and educational content.
7. Jinja2: Used to render HTML templates.
8. Uvicorn: Used to run the FastAPI application.
9. Python-dotenv: Used to load the API key and configuration from the environment file.

4. Main Features

1. AI Question and Answer

This feature allows students to ask academic questions and receive AI-generated answers. It helps students understand different topics.

Example: What is Artificial Intelligence?

2. Simple Explanation

This feature explains difficult topics in simple and understandable language. It helps students learn complex concepts more easily.

Example: Explain photosynthesis in simple words.

3. AI Quiz Generation

This feature generates multiple-choice questions based on a given topic. Students can use these quizzes to practise and test their knowledge.

Example: Create a quiz about the solar system.

4. Text Summarization

This feature converts long educational text into a shorter summary containing the main points. It helps students review important information.

Example: Summarize the water cycle.

5. Personalized Learning Path

This feature recommends learning steps based on the topic and the student's learning level. It helps students organize their learning.

Example: Give me a beginner learning path for Python.

5. System Architecture

EduGenie follows a client-server architecture.

Frontend: HTML, CSS, and JavaScript are used to create the user interface. Students can enter questions and select the required feature.

Backend: Python and FastAPI receive user requests and process them through the appropriate modules.

AI Processing: The Gemini API generates answers, explanations, quizzes, summaries, and learning recommendations. An optional local model can be used for explanations.

Output: The generated response is sent back to the frontend and displayed on the web page.

6. Project Workflow

1. The student opens the EduGenie web application.
2. The student selects a feature.
3. The student enters a question or educational text.
4. JavaScript sends the request to the FastAPI backend.
5. The backend processes the request using the relevant Python module.
6. The module sends the prompt to the Gemini API or uses the configured local model.
7. The AI generates the requested response.
8. The backend returns the response to the frontend.
9. The result is displayed on the web page.

7. Project Folder Structure

EduGenie/

- main.py
- ai_client.py
- qna.py
- explanation_module.py
- quiz_module.py
- summary_module.py
- learning_path.py
- requirements.txt
- .env
- .gitignore
- README.md
- templates/
  - index.html
- static/
  - style.css
- tests/
  - test_quiz.py

Important Files

main.py: Creates the FastAPI application and defines the API endpoints.

ai_client.py: Connects the application to the Gemini API.

qna.py: Handles question-and-answer requests.

explanation_module.py: Handles simple explanations.

quiz_module.py: Generates and processes quizzes.

summary_module.py: Handles text summarization.

learning_path.py: Generates learning recommendations.

index.html: Contains the structure of the web page.

style.css: Controls the design and appearance of the web page.

.env: Stores the Gemini API key and application configuration.

8. API Endpoints

- GET / : Opens the EduGenie home page.
- POST /qa : Answers students' questions.
- POST /explain : Explains topics in simple language.
- POST /quiz : Generates quizzes.
- POST /summarize : Summarizes educational text.
- POST /learn/recommendations : Provides learning recommendations.
- GET /docs : Displays interactive API documentation.

9. Gemini API Key

EduGenie uses the Google Gemini API to generate AI-based educational content.

The API key is created through Google AI Studio. It is stored in the .env file and used by the backend to communicate with the Gemini model.

Example configuration:

GEMINI_API_KEY=YOUR_API_KEY
GEMINI_MODEL=gemini-2.5-flash
USE_LOCAL_EXPLAINER=false

The API key must be kept private and should not be included in frontend code.

10. How to Run the Project

Step 1: Open the EduGenie project folder in Visual Studio Code.

Step 2: Open the terminal and create a virtual environment.

python -m venv .venv

Step 3: Activate the virtual environment.

.venv\Scripts\activate

Step 4: Install the required packages.

pip install -r requirements.txt

Step 5: Add the Gemini API key to the .env file.

Step 6: Start the application.

uvicorn main:app --reload

Step 7: Open the following URL in a browser.

http://127.0.0.1:8000

To access the API documentation, open:

http://127.0.0.1:8000/docs

11. Advantages

- Provides AI-powered educational support.
- Combines multiple learning features in one application.
- Helps students understand difficult topics.
- Supports quiz-based practice.
- Provides learning recommendations.
- Offers a simple web-based interface.

12. Limitations

- Gemini-powered features require an internet connection.
- A valid Gemini API key is required.
- API usage may have limits or charges.
- AI-generated answers may sometimes be inaccurate.
- The optional local model may require additional computer resources.

13. Future Enhancements

- Student login and account management.
- Learning progress tracking.
- Saving quiz scores and results.
- Support for additional languages.
- More quiz types and difficulty levels.
- A dashboard to monitor learning progress.

These are possible future improvements and are not necessarily available in the current version.

14. Conclusion

EduGenie is an AI-powered educational web application developed using Python, FastAPI, HTML, CSS, JavaScript, and the Google Gemini API. It provides question answering, simple explanations, quiz generation, text summarization, and personalized learning recommendations.

The main objective of this project is to make education more accessible, interactive, and easier to understand. EduGenie helps students learn topics, practise questions, and organize their studies through a single web application.
