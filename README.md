README FILE

This is a Python-based Task Manager application that allows users to manage tasks, including adding, updating, deleting, and viewing tasks. The tasks are stored in a JSON file for persistence.

Features
Add new tasks with descriptions, deadlines, and priorities (low, medium, high).
View tasks based on various filters like status (pending/completed) and priority.
Update tasks by changing the description, priority, or marking them as completed.
Delete tasks by their ID.
Task data is saved in a tasks_storage.json file.
File Overview
tasks_storage.json: Stores all tasks in JSON format.
task_manager.py: Main script containing all logic and functionality for managing tasks.

id: Unique identifier for each task.
description: A brief description of the task.
deadline: Task deadline in YYYY-MM-DD format.
priority: The priority level of the task (low, medium, high).
status: The current status of the task (pending or completed).
Task Methods:
to_dict(): Used to Convert the task object into a dictionary format suitable for JSON storage.
Task Manager Class
The TaskManager class handles all operations:

load_tasks(): Loads tasks from the tasks_storage.json file.
save_tasks(): Saves all tasks back to the JSON file.
add_task(description, deadline, priority): Adds a new task.
view_tasks(status=None, priority=None): Displays tasks with optional filters for status and priority.
update_task(task_id, new_description=None, mark_completed=False, new_priority=None): Updates the task with new details or marks it as completed.
delete_task(task_id): Deletes a task by ID.
Task Viewing Menu
The task viewing menu allows users to filter and view tasks:

View all tasks.
View only pending tasks.
View only completed tasks.
View tasks filtered by priority (low, medium, high).
How to Use the Program
Add Task: Add a new task with its description, deadline, and priority.
View Tasks: View tasks based on status (pending/completed) or priority (low/medium/high).
Update Task: Update a task by modifying its description, priority, or status.
Delete Task: Delete a task by providing its ID.
Example Usage:
bash
Copy
Edit
Task Manager
1. Add Task
2. View Tasks
3. Update Task
4. Delete Task
5. Exit

