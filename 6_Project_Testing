Phase 6 – Project Testing
FitBuddy – AI-Powered Personalized Fitness Assistant
Template folder: 6.Project Testing
Phase Objective
Verify the core application endpoints, validation behavior, startup behavior, and AI fallback paths.

6.1 Existing Automated Tests
• test_health verifies GET /health returns HTTP 200 and a status value of ok.
• test_profile_validation verifies invalid profile input returns HTTP 422.

6.2 Functional Test Cases
• Create profile with valid values fi profile should be stored and an ID returned.
• Retrieve valid profile ID fi profile details should be returned.
• Retrieve unknown profile ID fi HTTP 404 should be returned.
• Generate rule-based plan fi plan should reflect the user's stated goal.
• Generate AI plan without API key fi local-fallback response should be returned.
• Generate nutrition without API key fi local nutrition response should be returned.
• Submit rating outside 1–5 fi validation should reject the request.
• Submit valid feedback fi feedback ID and confirmation should be returned.
• Call admin endpoint with invalid token fi HTTP 401 should be returned.
• Call admin endpoint with valid configured token fi profiles and feedback can be returned.

6.3 AI-Specific Testing
• Verify Gemini is called only when the API key is configured.
• Verify nutrition output is valid JSON with daily_habits and meal_ideas.
• Verify exceptions from Gemini do not crash the API and trigger fallback behavior.
• Verify feedback-driven revision does not replace the plan when the revision call fails.

6.4 Current Test Scope
• The supplied project currently includes basic automated health and validation tests.
• Additional endpoint, database, AI success/failure, authorization, and integration tests are recommended before
production use.
Phase Deliverables
• Test cases
• Automated smoke tests
• AI failure tests
• Validation tests
• Test improvement plan
FitBuddy Files Related to This Phase
• tests/test_app.py
• app/routes.py
• app/schemas.py

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
