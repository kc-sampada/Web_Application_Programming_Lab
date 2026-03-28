LAB 1 — Personal Portfolio Website using HTML and CSS

1. Created a navigation bar with fixed positioning and links to each section of the page.
2. Built an About section with a profile photo and introduction text using a flex layout.
3. Added a Projects section displaying four project cards in a responsive grid layout.
4. Implemented an interactive Calendar using JavaScript to navigate between months and highlight the current date.
5. Created an Enquiry form with input fields for name, email, phone and message.
6. Added a Contact section and a footer at the bottom of the page.
7. Applied consistent CSS styling for colors, spacing, borders, and alignment throughout.

This portfolio was created to present personal information, projects, and contact details in a clean and organized format. A plain text or unformatted introduction can be difficult to read and does not leave a good impression. Using structured HTML sections makes it easier for visitors to navigate and find relevant information quickly. The fixed navbar allows smooth access to any section at any time without scrolling back to the top. The project cards were styled with a grid layout so that multiple projects can be viewed side by side in a readable way. The calendar was included to add an interactive element to the page and demonstrate JavaScript skills. The enquiry form provides a direct way for visitors to reach out. CSS styling such as background colors, border radius, box shadows, and hover effects were applied to improve the overall look and usability. Hence, the implementation improved structure, readability, and user experience of the portfolio.


LAB 2 — Intro to JavaScript

1. Demonstrated the difference between var, let and const with examples of scope and reassignment.
2. Created regular functions and arrow functions to show different ways of defining reusable logic.
3. Used objects to group related data and access properties using dot notation.
4. Applied the map() method to transform array elements into a new array.
5. Used the filter() method to extract elements from an array based on a condition.
6. Demonstrated the spread operator to combine arrays and copy objects.

This lab was done to build a foundational understanding of core JavaScript concepts. Without understanding var, let and const, it is easy to introduce bugs related to scope and accidental reassignment. Functions and arrow functions are essential building blocks used in every JavaScript project. Objects are necessary to represent real world data in a structured way. Map and filter are widely used array methods in modern JavaScript and React, so understanding them early is important. The spread operator simplifies working with arrays and objects without mutating the original data. Overall this lab helped establish the JavaScript skills needed for upcoming React labs.

LAB 3 — Login and Register Form with Custom Input Component (React)

1. Created a React project with separate Login and Register page components.
2. Built a reusable custom Input component to avoid repeating input field code.
3. Used React useState hook to manage form field values and error messages.
4. Added basic validation to check for empty fields and matching passwords on register.
5. Applied CSS styling for form layout, input fields and buttons.

This lab was done to learn how React state and components work together in a real use case. Building forms in plain HTML does not scale well when the same input fields are repeated across multiple pages. Creating a custom Input component made the code cleaner and reusable across both the login and register forms. Using useState to control form values introduced the concept of controlled components, which is the standard way of handling forms in React. Validation logic was added to give users clear feedback before submission. This lab built the practical skills needed to handle user input in React applications.

LAB 4 — CRUD Todo App (React)

1. Created a React app where users can add, view, edit and delete todo items.
2. Used useState to store and update the list of todos.
3. Implemented add functionality by capturing input and appending a new item to the state array.
4. Implemented delete functionality by filtering out the selected item from the state array.
5. Implemented edit functionality by replacing the selected item in the array with updated text.
6. Rendered the todo list dynamically from state using the map() method.

This lab was done to practice state manipulation in React through a practical CRUD application. Managing a list of items requires understanding how to add, update and remove entries from state without directly mutating it. Using filter for deletion and map for updates reinforced immutable state patterns that are essential in React. Rendering the list dynamically from state ensured the UI always reflected the current data. This lab strengthened the understanding of how React re-renders components when state changes, which is the core concept behind building interactive UIs.

LAB 5 — Login and Register with FastAPI Authentication (Backend)

1. Set up a FastAPI project with a clear folder structure separating routes, controllers, models and database connection.
2. Created a database connection file and configured it to connect to the database using SQLAlchemy.
3. Defined a User model with fields for id, name, email and hashed password.
4. Created and applied database migrations using Alembic to set up the users table.
5. Built a register route that accepts user details, hashes the password and saves the user to the database.
6. Built a login route that verifies credentials and returns a JWT access token on success.
7. Added authentication middleware to protect routes using the generated token.

This lab was done to learn how to build a secure authentication system in a real backend framework. Storing plain text passwords is a serious security risk, so hashing with bcrypt was necessary before saving to the database. Using JWT tokens for login allowed the backend to verify the identity of users on protected routes without storing session data on the server. Separating the code into controllers, models and routes followed standard backend architecture and made the code easier to maintain and scale. Migrations with Alembic ensured that database schema changes were tracked and reproducible. This lab established the backend foundation needed for the next lab.


LAB 6 — Todo API with User Authentication (FastAPI with ORM and Migrations)

1. Created a Todo model linked to the User model using a foreign key on user id.
2. Applied Alembic migrations to add the todos table to the database.
3. Built routes to create, read, update and delete todos for the authenticated user.
4. Used the JWT token from the login response to identify the current user on each request.
5. Filtered todo queries by user id so each user only sees their own todos.
6. Organized code into separate route and controller files following the structure from Lab 5.

This lab was done to extend the authentication system from Lab 5 into a fully functional protected API. Displaying all todos from the database regardless of user would be a privacy issue, so filtering by user id was necessary to ensure each user only accesses their own data. Using the authenticated user's id from the JWT token to scope database queries is the standard pattern in real world APIs. The foreign key relationship between todos and users enforced data integrity at the database level. Reusing the project structure from Lab 5 kept the codebase consistent and easy to navigate. This lab completed the full stack foundation by connecting a secure backend API to user-specific data.
