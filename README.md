# Task Buddy - Personal Task Manager

A comprehensive task management application built with Vue 3, featuring user authentication, CRUD operations, task sharing, and role-based access control (RBAC).

## Screenshots

![Screenshot 1](screenshots/screenshot1.png)
![Screenshot 2](screenshots/screenshot2.png)
![Screenshot 3](screenshots/screenshot3.png)
![Screenshot 4](screenshots/screenshot4.png)
![Screenshot 5](screenshots/screenshot5.png)
![Screenshot 6](screenshots/screenshot6.png)
![Screenshot 7](screenshots/screenshot7.png)
![Screenshot 8](screenshots/screenshot8.png)
![Screenshot 9](screenshots/screenshot9.png)
![Screenshot 10](screenshots/screenshot10.png)
![Screenshot 11](screenshots/screenshot11.png)
![Screenshot 12](screenshots/screenshot12.png)

## Features Implemented

### ✅ Core CRUD Operations
- **Add** tasks with name, category, priority, and due date
- **Read/View** all tasks with filtering by category
- **Update** tasks (edit functionality)
- **Delete** tasks

### ✅ User Accounts & Authentication
- User registration and login
- Session management
- Protected routes (authentication required)

### ✅ Task Categorization
- Personal
- Work
- School

### ✅ Priority Levels
- Low (green badge)
- Medium (yellow badge)
- High (red badge)

### ✅ Due Dates
- Date picker for setting task deadlines
- Visual display of due dates

### ✅ Task Sharing with RBAC
- Share tasks with other users
- **View Only** permission - users can see but not edit
- **Can Edit** permission - users can modify shared tasks
- Owner always has full control

### ✅ Accessibility Features
- ARIA labels on all form inputs
- Semantic HTML structure
- Keyboard navigation support
- Error messages with role="alert"
- High contrast design for visual impairment

## Design Considerations

### For Diverse Users
- **Visual Impairment**: ARIA labels, semantic HTML, high contrast colors
- **Busy Parents**: Quick add/edit, category filters, priority system
- **Students**: School category, due dates, simple interface

## Installation

```bash
npm install
npm run dev
```

## Usage

### Login Credentials
- Username: `admin` / Password: `admin123`
- Username: `user1` / Password: `user123`

Or register a new account.

### Adding Tasks
1. Fill in task name, select category, priority, and due date
2. Click "Add" button

### Editing Tasks
1. Click "Edit" on any task you own or have edit permission
2. Modify fields and click "Update"

### Sharing Tasks
1. Click "Share" on tasks you own
2. Select user and permission level (View/Edit)
3. Click "Share"

### Filtering
- Use category buttons to filter tasks by Personal, Work, or School

## Technology Stack
- Vue 3 (Composition API)
- Pinia (State Management)
- Vue Router (Navigation)
- Vite (Build Tool)

## Project Structure
```
src/
├── stores/
│   ├── auth.js      # User authentication
│   └── tasks.js     # Task management & RBAC
├── views/
│   ├── Login.vue    # Login/Register
│   └── Tasks.vue    # Main task interface
├── router/
│   └── index.js     # Route configuration
└── App.vue          # Root component
```
