# 📝 Notes App – CRUD Mini Project

A simple **Notes application** built using **Node.js, Express, and EJS** to practice **RESTful CRUD operations** without using a database.  
This project focuses on backend fundamentals, routing, middleware usage, and state management using in-memory data.

---

## 🚀 Features

- Create new notes
- View all notes
- View note details
- Edit existing notes
- Delete notes
- Pin / unpin notes
- Pinned notes move to the top
- Clean RESTful routes
- Server-side rendering using EJS
- Simple and responsive UI

---

## 🧠 What This Project Demonstrates

- REST API design using Express
- CRUD operations without a database
- Understanding of JavaScript object references
- Route handling with dynamic parameters
- Use of middleware like `method-override`
- Server-side rendering with EJS templates
- Basic UI styling with CSS

---

## 🛠️ Tech Stack

### Backend
- **Node.js**
- **Express.js**
- **UUID** (for unique note IDs)
- **Method-Override** (for PATCH & DELETE requests)

### Frontend
- **EJS** (templating engine)
- **HTML5**
- **CSS3**
- **Font Awesome** (icons)

### Data Storage
- In-memory JavaScript array (no database)

---

## 📁 Project Structure

```
NOTES-APP/
├── .github/
├── node_modules/
├── public/
│   ├── images/
│   └── stylesheets/
├── views/
│   ├── includes/
│   │   └── header.ejs
│   ├── edit.ejs
│   ├── error.ejs
│   ├── expand.ejs
│   ├── index.ejs
│   └── newNote.ejs
├── package.json
├── package-lock.json
├── readme.md
└── server.js
```


---

## 🔀 Routes Overview

| Method | Route | Description |
|------|------|-------------|
| GET | `/notes` | View all notes |
| GET | `/notes/new` | Create note page |
| POST | `/notes/new` | Add new note |
| GET | `/notes/:id` | View note details |
| GET | `/notes/:id/edit` | Edit note page |
| PATCH | `/notes/:id/edit` | Update note |
| DELETE | `/notes/:id` | Delete note |
| GET | `/notes/:id/pin` | Pin / unpin note |

---

## 📌 Pin Feature Logic

- Each note has an `isPinned` boolean flag
- Pinned notes are moved to the top of the list
- Clicking the pin icon toggles pin state
- UI updates visually using conditional CSS classes

---

@copyright 2026 Punit Sahu
