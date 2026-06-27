# Vertical AI Platform Backend

## Overview
The Vertical AI Platform backend is built using FastAPI and serves as the core of the application, providing APIs, business logic, and integration with AI functionalities. This backend is designed to support a modular and scalable architecture, enabling the development of industry-specific AI SaaS products.

## Directory Structure
- **app/**: Contains the main application logic.
  - **api/**: API endpoints and request handling.
  - **core/**: Core application logic and configuration.
  - **domain/**: Domain models and business logic.
  - **infrastructure/**: Database connections and external service integrations.
  - **services/**: Service classes encapsulating business logic.
  - **ai/**: AI-related functionalities and integrations.
  - **integrations/**: Code for integrating with external systems.
  - **workflows/**: Workflow definitions and orchestration logic.
  - **main.py**: Entry point of the application.

- **tests/**: Unit and integration tests for the backend application.

- **requirements.txt**: Lists Python dependencies required for the backend.

- **alembic.ini**: Configuration file for Alembic, used for database migrations.

## Setup Instructions
1. **Clone the Repository**
   ```bash
   git clone <repository-url>
   cd vertical-ai-platform/backend
   ```

2. **Create a Virtual Environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run Database Migrations**
   ```bash
   alembic upgrade head
   ```

5. **Start the Application**
   ```bash
   uvicorn app.main:app --host 0.0.0.0 --port 8000 --reload
   ```

## Testing
To run the tests, ensure your virtual environment is activated and execute:
```bash
pytest tests/
```

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any enhancements or bug fixes.

## License
This project is licensed under the MIT License. See the LICENSE file for details.