Phase 5 – Project Development Phase
FitBuddy – AI-Powered Personalized Fitness Assistant
Template folder: 5. Project Development Phase
Phase Objective
Implement the designed FitBuddy features as a working FastAPI application.

5.1 Backend Development
• FastAPI application created in app/main.py with application metadata and lifespan-based database initialization.
• Routes implemented in app/routes.py for profile management, workout generation, nutrition, feedback, AI plans, and
administration.
• Static files are mounted at /static and index.html is served at the root route.

5.2 Database Development
• SQLite database is created as fitbuddy.db.
• Tables for profiles, fitness_plans, and feedback are created automatically if they do not exist.
• Parameterized SQL statements are used for insert and lookup operations.

5.3 AI Development
• Gemini access is centralized through generate_gemini_text in app/ai_common.py.
• Workout generation requests a concise seven-day beginner-friendly plan with at least two recovery days.
• Nutrition generation requests strict JSON and validates the generated structure.
• Plan revision sends the profile, current plan, rating, and feedback back to Gemini.

5.4 Personalization and Fallbacks
• Rule-based workout logic adapts exercises to strength/muscle, weight/fat, or general goals.
• AI plan generation stores successful generated plans in SQLite.
• If GEMINI_API_KEY is missing or the AI request fails, the route returns a local starter plan.
• Nutrition also has a local fallback response.

5.5 Frontend Development
• The project contains app/templates/index.html as the main browser interface.
• The interface is served directly by FastAPI, keeping the project simple for local demonstration.
Phase Deliverables
• Working backend
• Database
• AI integration
• Fallback logic
• Frontend interface
FitBuddy Files Related to This Phase
• app/main.py
• app/routes.py
• app/database.py
• app/gemini_generator.py
• app/gemini_flash_generator.py
• app/updated_plan.py
• app/templates/index.html

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
