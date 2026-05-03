# Assignment 7: API Planning for To-Do List App

## Objective
To plan the necessary APIs for a To-Do List application, focusing on endpoints and logic.

## API Endpoints

### 1. Add Task (POST)
- **Endpoint:** `/api/tasks`
- **Body:** `{ "title": "string" }`
- **Logic:** Unique ID will be generated using `Date.now()`.

### 2. Read All Tasks (GET)
- **Endpoint:** `/api/tasks`
- **Response:** Returns an array of all task objects.

### 3. Update Task Status (PUT)
- **Endpoint:** `/api/tasks/:id`
- **Body:** `{ "completed": boolean }`
- **Logic:** Finds task by ID and toggles completion status.

### 4. Delete Task (DELETE)
- **Endpoint:** `/api/tasks/:id`
- **Logic:** Removes the task from the array based on ID.

## Potential Challenges
Data persistence is a challenge since we are using volatile memory (arrays) for now.
