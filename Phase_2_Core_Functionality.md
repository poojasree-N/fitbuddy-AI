# Phase 2 – Core Functionality Development

## Activity 2.1: Develop the Core Functionalities

### Workout Plan Generation
Function: `generate_workout_gemini()`

File: `gemini_generator.py`

Generates a personalized 7-day workout plan based on the user's goal and workout intensity.

### Nutrition Tip Generation
Function: `generate_nutrition_tip_with_flash()`

File: `gemini_flash_generator.py`

Generates a concise nutrition or recovery tip related to the user's fitness goal.

### Feedback-Based Plan Updating
Function: `update_workout_plan()`

File: `updated_plan.py`

Updates the existing workout plan based on user feedback.

### User and Plan Storage
File: `database.py`

Stores user information and generated workout plans using SQLite and SQLAlchemy.

## Activity 2.2: FastAPI Backend

- Receives user input from the HTML form.
- Validates input using Pydantic schemas.
- Connects routes with workout and nutrition functions.
- Stores user and plan information in the database.
