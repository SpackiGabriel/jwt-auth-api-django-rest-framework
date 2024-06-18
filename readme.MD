# Django Rest Framework Authentication API

This project is an authentication API using Django Rest Framework and dj-rest-auth.

## Available Endpoints

### Register User

- **URL:** `api/auth/register/`
- **Method:** `POST`
- **Description:** Registers a new user.
- **Example Request:**
  ```json
  {
    "username": "user",
    "password1": "password",
    "password2": "password",
    "email": "user@example.com"
  }
  ```

### Login

- **URL:** `api/auth/login/`
- **Method:** `POST`
- **Description:** Authenticates a user and returns access tokens.
- **Example Request:**
  ```json
  {
    "username": "user",
    "password": "password"
  }
  ```

### Logout

- **URL:** `api/auth/logout/`
- **Method:** `POST`
- **Description:** Logs out the authenticated user.

### User Details

- **URL:** `api/auth/user/`
- **Method:** `GET`
- **Description:** Returns details of the authenticated user.

### Verify Token

- **URL:** `api/auth/token/verify/`
- **Method:** `POST`
- **Description:** Verifies the validity of a token.
- **Example Request:**
  ```json
  {
    "token": "your-token"
  }
  ```

### Refresh Token

- **URL:** `api/auth/token/refresh/`
- **Method:** `POST`
- **Description:** Refreshes the access token.
- **Example Request:**
  ```json
  {
    "token": "your-token"
  }
  ```

## Installation and Setup

1. Clone the repository:
  ```bash
  git clone https://github.com/your-username/your-repo-name.git
  cd your-repo-name
  ```

2. Install Poetry if you haven't already:
  ```bash
  pip install poetry
  ```

3. Install the dependencies:
  ```bash
  poetry install
  ```

4. Apply migrations:
  ```bash
  poetry run python manage.py migrate
  ```

4. Run the development server:
  ```bash
  poetry run python manage.py runserver
  ```

## Usage

Use a tool like [Postman](https://www.postman.com/) or [httpie](https://httpie.io/) to interact with the API endpoints.

