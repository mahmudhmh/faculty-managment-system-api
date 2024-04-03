# Faculty Management System README

This Faculty Management System is built using Node.js, Express.js, and Mongoose. It allows users to manage students and courses within a faculty. The system provides various functionalities including getting all students, getting a student by ID, adding a new student, deleting a student by ID, getting all courses, getting a course by ID, deleting a course by ID, and adding a new course.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/mahmudhmh/faculty-management-system-api.git
   ```

2. Navigate to the project directory:

   ```bash
   cd faculty-management-system-api
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Set up your MongoDB database.

5. Rename `.env.example` to `.env` and provide the necessary environment variables like `DB_URL` for your MongoDB connection.

6. Run the application:

   ```bash
   nodemon server.js
   ```

## API Endpoints

### You can check the API Documentation from the link below.

- [API Documentation](https://documenter.getpostman.com/view/34024588/2sA35JzfBc#3028f8ae-2318-4f73-a27a-b3a2adcf79a8)

### Students

#### Get all students

- **GET /api/students**
  - Returns a list of all students.

#### Get student by ID

- **GET /api/students/:id**
  - Returns a specific student by ID.

#### Add new student

- **POST /api/students**
  - Adds a new student. Requires JSON payload with student details.

#### Delete student by ID

- **DELETE /api/students/:id**
  - Deletes a student by ID.

### Courses

#### Get all courses

- **GET /api/courses**
  - Returns a list of all courses.

#### Get course by ID

- **GET /api/courses/:id**
  - Returns a specific course by ID.

#### Add new course

- **POST /api/courses**
  - Adds a new course. Requires JSON payload with course details.

#### Delete course by ID

- **DELETE /api/courses/:id**
  - Deletes a course by ID.

## Example Usage

### Get all students

```bash
curl http://localhost:1312/api/students
```

### Get student by ID

```bash
curl http://localhost:1312/api/students/{id}
```

### Add new student

```bash
curl -X POST -H "Content-Type: application/json" -d '{"name": "John Doe", "dept": "OS"}' http://localhost:1312/api/students
```

### Delete student by ID

```bash
curl -X DELETE http://localhost:1312/api/students/{id}
```

### Get all courses

```bash
curl http://localhost:1312/api/courses
```

### Get course by ID

```bash
curl http://localhost:1312/api/courses/{id}
```

### Add new course

```bash
curl -X POST -H "Content-Type: application/json" -d '{"courseName": "Computer Science", "grade": "Very Good"}' http://localhost:1312/api/courses
```

### Delete course by ID

```bash
curl -X DELETE http://localhost:1312/api/courses/{id}
```

## Contributors

- [Mahmoud Hussien](https://github.com/mahmudhmh)

## License

This project is licensed under the [MIT License](LICENSE).
