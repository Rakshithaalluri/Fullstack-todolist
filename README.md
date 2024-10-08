# Project-Application-Todolist
## Todo Web Application

### Objective:
The objective of this project is to develop a Todo Web Application where users can manage their daily tasks by storing them and updating their status. The application supports user authentication, task management, and profile management.

### Technologies Used:
- **Frontend**: ReactJS
- **Backend**: Node.js, Express
- **Authentication**: JWT (JSON Web Tokens)
- **Unique ID Generation**: UUID
- **Database**: SQLite3

### Functional Requirements:

#### 1. User Authentication:
- Users can register using a **Signup** feature by providing necessary details.
- Registered users can log in using a **Login** feature, which authenticates them via **JWT tokens**.
- All secured API routes are protected and accessible only after validating the user's JWT token.

#### 2. Todo Management (CRUD Operations):
- Users can **Create, Read, Update, and Delete** (CRUD) their daily tasks.
- Tasks can have various statuses such as **done**, **pending**, **in progress**, or **completed**.
- Users can update the status of each task.

#### 3. User Profile Management:
- Users can manage their profile by updating their name, email, and password.
- Profile management features are secured and accessible only to authenticated users.

### Setup Instructions:

1. **Frontend Setup (ReactJS)**
   - Navigate to the `frontend` folder.
   - Install dependencies:
     ```bash
     npm install
     ```
   - Start the development server:
     ```bash
     npm start
     ```

2. **Backend Setup (Node.js, Express)**
   - Navigate to the `backend` folder.
   - Install dependencies:
     ```bash
     npm install
     ```
   - Start the server:
     ```bash
     npm run dev
     ```
   - The backend will run on `http://localhost:3000` by default.

### API Endpoints:

#### Authentication:
- `POST /register`: Register a new user.
- `POST /login`: Login and receive a JWT token.

#### Todo Management:
- `GET /todos`: Retrieve all tasks (requires authentication).
- `POST /todos`: Add a new task (requires authentication).
- `PUT /todos/:id`: Update an existing task (requires authentication).
- `DELETE /todos/:id`: Delete a task (requires authentication).

#### User Profile:
- `GET /profile`: Retrieve user profile (requires authentication).
- `PUT /profile`: Update user profile (requires authentication).

