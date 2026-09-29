Phase 4 – Project Planning Phase
FitBuddy – AI-Powered Personalized Fitness Assistant
Template folder: 4. Project Planning Phase
Phase Objective
Plan implementation activities, dependencies, environment setup, testing, deployment, and phase deliverables.

4.1 Development Plan
• Step 1: Prepare the Python environment and install requirements.
• Step 2: Build the FastAPI application and database initialization.
• Step 3: Implement profile creation and retrieval.
• Step 4: Implement rule-based workout generation.
• Step 5: Integrate Gemini workout generation.
• Step 6: Integrate nutrition generation and JSON validation.
• Step 7: Add feedback storage and feedback-driven plan revision.
• Step 8: Add tests and health validation.
• Step 9: Prepare Render deployment configuration and project documentation.

4.2 Technology Plan
• Python is used as the primary programming language.
• FastAPI and Uvicorn provide the web/API layer and development server.
• SQLite provides lightweight local persistence.
• Pydantic provides request validation.
• google-genai provides access to Gemini generation.
• HTML provides the browser interface.
• Render is configured as a deployment target.

4.3 Environment Plan
• requirements.txt contains fastapi, uvicorn[standard], and google-genai.
• .env.example defines Gemini API key, model names, admin token, and application environment.
• The actual .env file should remain private and must not be committed or included in public documentation.

4.4 Risk and Mitigation Plan
• Gemini unavailable fi return a local fallback workout or nutrition response.
• Invalid user input fi reject the request through Pydantic validation.
• Missing profile fi return HTTP 404.
• Unauthorized admin access fi require a matching admin token.
• AI returns invalid nutrition structure fi validate parsed JSON and fall back to default nutrition.
Phase Deliverables
• Implementation schedule
• Technology plan
• Environment plan
• Risk/mitigation plan
FitBuddy Files Related to This Phase
• requirements.txt
• .env.example
• README.md
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
Render configuration in render.yaml
