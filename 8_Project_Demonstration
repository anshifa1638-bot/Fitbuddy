Phase 8 – Project Demonstration
FitBuddy – AI-Powered Personalized Fitness Assistant
Template folder: 8.Project Demonstration
Phase Objective
Provide a clear end-to-end demonstration script showing the major FitBuddy features and the role of Generative AI.

8.1 Demonstration Setup
• Open the FitBuddy project in VS Code.
• Ensure dependencies are installed.
• Configure .env with GEMINI_API_KEY for the AI demonstration.
• Run uvicorn app.main:app --reload.
• Open http://127.0.0.1:8000.

8.2 Demonstration Flow
• Step 1 – Show the FitBuddy home page.
• Step 2 – Enter a sample profile with name, age, height, weight, and fitness goal.
• Step 3 – Create the profile and show the stored profile ID.
• Step 4 – Generate the rule-based workout plan.
• Step 5 – Generate the Gemini seven-day AI plan.
• Step 6 – Show nutrition recommendations and meal ideas.
• Step 7 – Submit a 1–5 rating and feedback message.
• Step 8 – Explain that feedback can trigger an updated plan when the required conditions are available.
• Step 9 – Show the health endpoint and, if configured, the protected admin endpoint.
• Step 10 – Explain the fallback behavior by demonstrating the application without a Gemini key or when AI generation
is unavailable.

8.3 Points to Explain During Viva/Demo
• Why FastAPI was selected: simple Python API development and automatic API schema support.
• Why Gemini is used: natural-language generation enables personalized workout and nutrition guidance.
• Why SQLite is used: lightweight local persistence suitable for the prototype.
• Why fallback logic is included: the application should still provide useful starter guidance when AI is unavailable.
• How feedback improves the system: feedback is stored and can be passed with the previous plan to Gemini for
revision.

8.4 Expected Demonstration Result
• The evaluator can see a complete flow from user profile fi plan generation fi nutrition fi feedback fi potential plan
revision, with data persisted locally.
Phase Deliverables
• Demo script
• Feature walkthrough
• Viva explanation points
• Expected output
FitBuddy Files Related to This Phase
• app/templates/index.html
• app/routes.py
• app/database.py
• app/gemini_generator.py
• app/gemini_flash_generator.py
• app/updated_plan.py
• tests/test_app.py

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
