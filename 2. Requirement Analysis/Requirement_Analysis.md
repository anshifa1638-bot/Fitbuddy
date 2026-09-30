Phase 2 – Requirement Analysis
FitBuddy – AI-Powered Personalized Fitness Assistant
Template folder: 2. Requirement Analysis
Phase Objective
Translate the FitBuddy idea into functional, non-functional, input, output, and technology requirements.

2.1 Functional Requirements
• Create a user profile with name, age, height, weight, and fitness goal.
• Retrieve an existing profile by profile ID.
• Generate a rule-based workout plan according to the stated goal.
• Generate a Gemini-based seven-day workout plan.
• Provide nutrition recommendations and meal ideas.
• Store feedback with a rating from 1 to 5 and a message.
• Use feedback to revise the latest plan when Gemini configuration and a previous plan are available.
• Provide an admin endpoint for viewing profiles and associated feedback.

2.2 Non-Functional Requirements
• The application should be easy to run locally with Python and Uvicorn.
• Inputs must be validated before being processed.
• API secrets must be provided through environment variables.
• The application should degrade gracefully when Gemini is unavailable.
• The code should separate routing, database, schemas, configuration, and AI generation responsibilities.

2.3 Input Requirements
• Profile: name, age, height_cm, weight_kg, goal.
• Feedback: optional profile_id, rating, message.
• Environment configuration: GEMINI_API_KEY, model names, and ADMIN_TOKEN.

2.4 Output Requirements
• Profile records and generated profile IDs.
• Structured local workout plans.
• Seven-day AI-generated workout text.
• Nutrition JSON containing guidance, daily habits, and meal ideas.
• Feedback confirmation and optional revised plan.
• Health-check response with application status.
Phase Deliverables
• Functional requirements
• Non-functional requirements
• Input/output specification
• Environment requirements
FitBuddy Files Related to This Phase
• app/schemas.py
• app/routes.py
• app/config.py
• .env.example
• requirements.txt

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
