````markdown
# Todo App

A simple and beginner-friendly **Todo App** built using **HTML, CSS, and JavaScript**.

This project allows users to add, edit, and delete tasks. The tasks are stored in the browser's **Local Storage**, so they remain available even after refreshing the page.

## Features

- Add new tasks
- Edit existing tasks
- Save edited tasks
- Delete tasks
- Prevent empty tasks from being added
- Store tasks in Local Storage
- Automatically load saved tasks after refreshing the page
- Simple and responsive user interface
- Gradient background with a simple modern design

## Technologies Used

- **HTML5** - Used to create the structure of the application
- **CSS3** - Used for styling and layout
- **JavaScript** - Used for task management and application functionality
- **Local Storage** - Used to store tasks in the browser

## How It Works

### 1. Adding a Task

The user enters a task in the input field and clicks the **Add** button.

JavaScript creates a task object containing:

```javascript
{
    id: Date.now(),
    text: "Task name"
}
````

The task is then added to the tasks array and saved in Local Storage.

### 2. Displaying Tasks

The `showTasks()` function displays all tasks from the tasks array.

JavaScript dynamically creates:

* A `div` for the task
* A `span` for the task text
* An **Edit** button
* A **Delete** button

### 3. Editing a Task

When the user clicks **Edit**:

* The task text becomes editable.
* The cursor is placed inside the task.
* The button changes from **Edit** to **Save**.

When the user clicks **Save**:

* Editing is disabled.
* The updated text is stored in the tasks array.
* The updated array is saved to Local Storage.

### 4. Deleting a Task

When the user clicks the delete icon:

* The selected task is removed from the tasks array.
* The updated array is saved to Local Storage.
* The task is removed from the page.

### 5. Local Storage

The application uses:

```javascript
localStorage.setItem()
```

to save tasks.

It uses:

```javascript
localStorage.getItem()
```

to retrieve saved tasks.

Because Local Storage stores data as strings, the project uses:

```javascript
JSON.stringify()
```

to convert the array into a string and:

```javascript
JSON.parse()
```

to convert it back into a JavaScript array.

## Project Structure

```text
Todo-App/
│
├── index.html
└── README.md
```

The HTML file contains the:

* HTML structure
* CSS styling
* JavaScript functionality

## How to Run

1. Download or clone the project.

2. Open the project folder.

3. Open `index.html` in any modern web browser.

4. Enter a task in the input box.

5. Click **Add**.

6. Use **Edit** to modify a task.

7. Use the delete icon to remove a task.

## Learning Concepts

This project demonstrates several important beginner JavaScript concepts:

* Variables
* Arrays
* Objects
* Functions
* `for` loops
* `if` conditions
* Event listeners
* DOM manipulation
* `createElement()`
* `appendChild()`
* `classList`
* `setAttribute()`
* `innerText`
* Array operations
* Local Storage
* JSON
* `JSON.stringify()`
* `JSON.parse()`

## Future Improvements

Some features that can be added in the future:

* Mark tasks as completed
* Add a Clear All button
* Add task categories
* Add task deadlines
* Add search functionality
* Add dark mode
* Add task filtering
* Improve mobile UI

## Author

**Tarak Sai**

This project was created as a beginner-friendly JavaScript practice project to understand **DOM manipulation, events, arrays, objects, and Local Storage**.

```
```
