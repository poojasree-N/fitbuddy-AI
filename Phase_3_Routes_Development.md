# Phase 3 – Routes Development

## Activity 3.1: Writing the Main Application Logic in routes.py

The `routes.py` file contains the main routing logic of the FitBuddy application. It connects the frontend, AI generation functions, feedback update function, and database operations.

## Core Routes

### 1. Home Route
Route:
`/`

- Displays the user form using `index.html`.
- Provides the input page for users.

### 2. Generate Workout Route
Route:
`/generate-workout`

- Receives user input using FastAPI Form parameters.
- Processes name, age, weight, goal, and intensity.
- Generates the workout plan.
- Generates the nutrition tip.
- Saves user details and the generated plan.
- Displays the result in `result.html`.

### 3. Submit Feedback Route
Route:
`/submit-feedback`

- Receives the user ID and feedback.
- Retrieves the original workout plan.
- Updates the plan using `update_workout_plan()`.
- Saves the updated plan in the database.
- Displays the updated result.

### 4. View All Users Route
Route:
`/view-all-users`

- Retrieves users and workout plans from the database.
- Displays them in `all_users.html`.
- Allows the admin to view user details and plans.

## Backend Flow

User Input → FastAPI Route → AI Function → Database → HTML Result
