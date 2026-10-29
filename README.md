# Employee Management System

A simple admin dashboard built with React to manage employee records.
Add employees with their department, role and salary, then edit or delete them anytime.
The home page shows live statistics.

Live demo: <un netlify link></un>[staffdesk-dashboard.netlify.app](https://staffdesk-dashboard.netlify.app/)

## Features

- Add, view, edit and delete employees
- Role list changes based on the selected department (IT, Sales or HR)
- Live statistics: total employees, departments, active and not active
- Form validation with messages
- Confirmation before deleting an employee
- Data is saved in the browser, so it stays after a refresh
- Neumorphism style design

## Built with

- React
- Vite
- Context API and React Hooks (useState, useEffect)
- CSS
- Browser localStorage
-

## Project structure

```
employee-management-system/
├── src/
│   ├── components/
│   │   ├── AddEmployee.jsx, AddEmployee.css
│   │   ├── EmployeeDetails.jsx, EmployeeDetails.css
│   │   ├── Header.jsx, Header.css
│   │   └── Navbar.jsx, Navbar.css
│   ├── context/
│   │   └── PageContext.jsx
│   ├── App.jsx, App.css
│   ├── Home.jsx
│   ├── Intro.jsx, Intro.css
│   ├── index.css
│   └── main.jsx
├── .gitignore
├── eslint.config.js
├── index.html
├── package.json
├── vite.config.js
└── README.md
```

## Run it yourself

1. Clone the repo
   ```
   git clone https://github.com/<un-username>/employee-management-system.git
   ```
2. Go into the folder and install the packages
   ```
   cd employee-management-system
   npm install
   ```
3. Start the app
   ```
   npm run dev
   ```
4. Open `http://localhost:5173` in your browser.

## How it works

- `PageContext` stores the current page, the employee being edited and the statistics, so every component can use them.
- Employees are saved in `localStorage` under the key `employee`.
- When an employee is added, edited or deleted, an `employeesUpdated` event updates the list and the statistics.

## What I learned

- Sharing state between components with Context API
- Building add, edit and delete features (CRUD) in React
- Dependent dropdowns, where the role list depends on the department
- Saving and reading data with localStorage

## Author

Joel Franklin
