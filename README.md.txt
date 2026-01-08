# HD Recipe Manager

A simple full-stack Recipe Manager project — lightweight front-end (HTML/CSS/JS) with a Node.js and Express backend.  
This project allows users to add, view, and remove recipes. It is ideal as a demo project or a starter application for learning CRUD operations using JavaScript.

## Features
- Add new recipes (title, ingredients, instructions, image URL)
- View a list of recipes and individual recipe details
- Delete recipes
- Static frontend with client-side JavaScript communicating with an Express backend

## Tech Stack
- **Frontend:** HTML, CSS, Vanilla JavaScript
- **Backend:** Node.js, Express
- **Data Storage:** JSON file or in-memory store (see `backend/model.js`)

## Repository Structure
HD-recipe-manager/
├─ backend/
│ ├─ server.js
│ ├─ routes.js
│ ├─ model.js
│ └─ package.json
└─ frontend/
├─ index.html
├─ recipe-store.html
├─ add-recipe.html
├─ show-recipe.html
├─ script.js
├─ styles.css
└─ assets/ (images)

shell
Copy code

> **Note:**  
> If the backend bundles the frontend, the Express server may serve the static files directly.  
> Otherwise, open `frontend/index.html` in a browser or serve the `frontend` folder using a static server such as `live-server` or `http-server`.

## Prerequisites
- Node.js (v14 or higher recommended)
- npm (included with Node.js)

## Installation & Running the Project

### 1. Clone the repository
```bash
git clone <your-repo-url>
cd HD-recipe-manager/HD-recipe-manager/backend
2. Install backend dependencies
bash
Copy code
npm install
3. Start the backend server
If package.json has a start script:

bash
Copy code
npm start
Otherwise:

bash
Copy code
node server.js
4. Open the frontend
If the backend serves the frontend, open:

arduino
Copy code
http://localhost:3000
(or the port shown in the terminal)

Otherwise, open the frontend manually:

bash
Copy code
HD-recipe-manager/frontend/index.html
Or run a simple static server:

bash
Copy code
# from the frontend folder
npx http-server . -p 8080
Then open:

arduino
Copy code
http://localhost:8080