Phase 3 – Project Design Phase
FitBuddy – AI-Powered Personalized Fitness Assistant
Template folder: 3. Project Design Phase
Phase Objective
Define the architecture, modules, database structure, API design, and AI workflow used by FitBuddy.

3.1 System Architecture
• Browser UI fi FastAPI routes fi validation/business logic fi SQLite persistence and/or Gemini services.
• The route layer selects between deterministic fallback logic and Gemini generation depending on configuration and
service availability.
• Feedback can flow back into Gemini to produce a revised workout plan.

3.2 Main Modules
• app/main.py – creates the FastAPI application, initializes the database, mounts static files, and exposes the root and
health endpoints.
• app/routes.py – contains profile, workout, AI plan, nutrition, feedback, and admin routes.
• app/database.py – creates SQLite tables and performs profile, plan, and feedback persistence.
• app/schemas.py – validates incoming profile and feedback data with Pydantic.
• app/config.py – loads environment variables and model configuration.
• app/ai_common.py – provides the common Gemini generation function.
• app/gemini_generator.py – generates workout plans.
• app/gemini_flash_generator.py – generates and validates nutrition JSON.
• app/updated_plan.py – revises a plan using user feedback.
3.3 Database Design

• profiles: id, name, age, height_cm, weight_kg, goal, created_at.
• fitness_plans: id, name, plan, created_at.
• feedback: id, profile_id, rating, message, created_at.

3.4 API Design
• GET /health – application health check.
• POST /profiles – create profile.
• GET /profiles/{profile_id} – retrieve profile.
• POST /profiles/{profile_id}/workout-plan – rule-based plan.
• POST /profiles/{profile_id}/ai-plan – Gemini plan with fallback.
• GET /profiles/{profile_id}/nutrition – nutrition guidance.
• POST /feedback – save feedback and optionally revise a plan.
• GET /admin/users – protected profile/feedback view.
Phase Deliverables
• Architecture design
• Module design
• Database design
• API design
• AI workflow
FitBuddy Files Related to This Phase
• app/main.py
• app/routes.py
• app/database.py
• app/models.py
• app/schemas.py
• app/ai_common.py

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
