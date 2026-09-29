Phase 7 – Project Documentation
FitBuddy – AI-Powered Personalized Fitness Assistant
Template folder: 7.Project Documentation
Phase Objective
Document how FitBuddy is structured, configured, run, tested, and deployed so another user can reproduce the project.

7.1 Project Structure
• app/ contains the application source code.
• app/templates/ contains the main HTML interface.
• app/static/ is the static-file directory.
• tests/ contains automated tests.
• fitbuddy.db is the local SQLite database.
• requirements.txt defines Python dependencies.
• .env.example defines required configuration variables.
• render.yaml defines hosted deployment settings.
• README.md contains local run and deployment guidance.

7.2 Local Run Procedure
• Open the project in VS Code.
• Create/activate a Python virtual environment.
• Install dependencies with pip install -r requirements.txt.
• Copy .env.example to .env and provide GEMINI_API_KEY if AI generation is required.
• Start with uvicorn app.main:app --reload.
• Open http://127.0.0.1:8000 in a browser.

7.3 Configuration
• GEMINI_API_KEY – Gemini authentication secret.
• FITBUDDY_WORKOUT_MODEL – workout generation model.
• FITBUDDY_TIP_MODEL – nutrition generation model.
• ADMIN_TOKEN – protects the admin endpoint.
• APP_ENV – application environment indicator.

7.4 Documentation Standards
• Keep secrets out of source control.
• Document new API endpoints when features are added.
• Update requirements.txt when dependencies change.
• Update test cases when route behavior changes.
• Keep deployment configuration synchronized with environment variables.
Phase Deliverables
• User/setup guide
• API summary
• Configuration guide
• Project structure guide
• Deployment guide
FitBuddy Files Related to This Phase
• README.md
• .env.example
• requirements.txt
• render.yaml

Project Technology
Component
Implementation
Backend
Frontend
Database
Generative AI
Validation
Testing
Python + FastAPI + Uvicorn
HTML/Jinja-style template served by FastAPI
SQLite using Python sqlite3
Google Gemini through google-genai
Pydantic
FastAPI TestClient
Deployment
Render configuration in render.yam
