# TeamCollab

TeamCollab is a project management tool that allows teams to collaborate on projects. This project includes an API to manage users, projects, tasks, and comments. The API is consumed by both a front-end web application and a mobile application.

## Setup Instructions

### Prerequisites

- Python 3.x
- pip (Python package installer)

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/teamcollab.git
    cd teamcollab
    ```

2. Create and activate a virtual environment:
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. Install the dependencies:
    ```sh
    pip install -r requirements.txt
    ```

### Database Migration

1. Apply migrations:
    ```sh
    python manage.py migrate
    ```

### Run the Server

1. Start the development server:
    ```sh
    python manage.py runserver
    ```

### API Documentation

- Swagger UI: [http://127.0.0.1:8000/swagger/](http://127.0.0.1:8000/swagger/)
- ReDoc: [http://127.0.0.1:8000/redoc/](http://127.0.0.1:8000/redoc/)

### API Root
The default basic root view for DefaultRouter

GET /api/
HTTP 200 OK
:Allow GET, HEAD, OPTIONS
Content-Type: application/json
Vary: Accept

{
    "users": "http://127.0.0.1:8000/api/users/",
    "projects": "http://127.0.0.1:8000/api/projects/",
    "project-members": "http://127.0.0.1:8000/api/project-members/",
    "tasks": "http://127.0.0.1:8000/api/tasks/",
    "comments": "http://127.0.0.1:8000/api/comments/"
}

