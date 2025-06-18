
# Simple REST API with Express and Joi

This is a basic RESTful API built with **Node.js**, **Express**, and **Joi** for data validation. The API manages a list of courses with CRUD operations (Create, Read, Update, Delete).

## Features

- List all courses
- Get a specific course by ID
- Add a new course
- Update an existing course
- Delete a course
- Input validation using Joi

## Getting Started

### Prerequisites

- Node.js installed on your machine
- npm (Node Package Manager)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/murilocardoso7/your-repo-name.git
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Run the application:
   ```bash
   node index.js
   ```

4. The server will start on port 3000 (or the port specified in `process.env.PORT`).

## API Endpoints

| Method | Endpoint           | Description                     |
| ------ | ------------------ | ------------------------------- |
| GET    | `/`                | Returns a simple "Hello, World" message |
| GET    | `/api/courses`     | Returns all courses             |
| GET    | `/api/courses/:id` | Returns a course by ID          |
| POST   | `/api/courses`     | Creates a new course            |
| PUT    | `/api/courses/:id` | Updates an existing course      |
| DELETE | `/api/courses/:id` | Deletes a course                |

## Validation

- Course names must be at least 3 characters long.
- Validation is performed using Joi.

## Example Request

To create a new course:

```bash
POST /api/courses
Content-Type: application/json

{
  "name": "New Course"
}
```

## License

This project is open source and available under the [MIT License](LICENSE).
