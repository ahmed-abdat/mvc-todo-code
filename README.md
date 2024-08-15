# TodoMVC React-Redux Challenge

## Project Overview

This project is a solution for a coding challenge that involves enhancing a TodoMVC application built with **React** and **Redux**. The challenge required implementing three main features:

1. **Delete a Task:** Implemented functionality to delete individual todo items.
2. **Filter Tasks:** Added filtering capability to display all, active, or completed tasks.
3. **Clear All Completed Tasks:** Implemented a feature to clear all completed tasks from the list.

## Challenge Solution

### 1. Delete a Task

- **Action:** Created a `deleteTodo` action that dispatches a `DELETE_TODO` action with the todo's `id` as a payload.
- **Reducer:** Updated the `todos` reducer to handle `DELETE_TODO` by filtering out the specified todo item.
- **Component Integration:** Connected the `deleteTodo` action to the relevant component, allowing users to delete tasks via the UI.

### 2. Filter Tasks

- **Selector:** Extended the `getFilteredTodos` selector to filter todos based on their completion status (all, active, completed).
- **Component Integration:** Integrated the filtering logic into the UI, enabling users to view tasks based on their status.

### 3. Clear All Completed Tasks

- **Action:** Created a `clearCompleted` action that dispatches a `CLEAR_COMPLETED` action.
- **Reducer:** Updated the `todos` reducer to handle `CLEAR_COMPLETED` by removing all completed tasks from the state.
- **Component Integration:** Connected the `clearCompleted` action to the UI, allowing users to clear completed tasks with a single click.

## Installation and Usage

1. **Install Dependencies:**

   ```bash
1. npm install
2. npm run dev
browser:
1. http://localhost:8080/#/
