## Introduction
Taskflow is a web-based to-do list application designed to help users manage their tasks efficiently. It allows users to create and delete tasks.

### Dependencies

The app requires two dependencies: Express.js and Body-Parser. Express.js is used to create the web server, and Body-Parser is used to parse the data sent from the client.

### Routes

The app has three routes:

1. **"/addtask"**: This route is used to add a new task to the list. When a user submits a new task, the app receives the data and adds it to the `task` array. The user is then redirected to the root URL (`"/"`) to see the updated list.
2. **"/removetask"**: This route is used to remove a task from the list. When a user checks a task, the app receives the data and removes the task from the `task` array and adds it to the `complete` array. The user is then redirected to the root URL (`"/"`) to see the updated list.
3. **"/"**: This route is used to render the EJS template and display the list of tasks and completed tasks.

### Templates

The app uses EJS (Embedded JavaScript) templates to render the HTML pages. The `index.ejs` template is used to display the list of tasks and completed tasks.

### Data Storage

The app stores the tasks and completed tasks in two arrays: `task` and `complete`. These arrays are used to store the data temporarily until it is persisted to a database or file.

### Running the App

To run the app, simply execute the `index.js` file using Node.js. The app will start listening on port 3000, and you can access it by navigating to `http://localhost:3000` in your web browser.

---
