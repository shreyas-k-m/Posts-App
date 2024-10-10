
# Posts App

This is a simple **Posts App** built with Node.js and Express. The app allows users to create, view, edit, and delete posts. Each post contains a `username` and `content`, and they are displayed in a dynamic, responsive user interface using EJS templates.

## Here is the Working link
https://quora-basic.onrender.com

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Routes](#routes)
- [Technologies](#technologies)
- [License](#license)

## Features
- View all posts
- Create a new post
- View individual post details
- Edit an existing post
- Delete a post

## Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/posts-app.git
    cd posts-app
    ```

2. **Install dependencies:**
    Make sure you have [Node.js](https://nodejs.org) installed. Then run:
    ```bash
    npm install
    ```

3. **Run the server:**
    ```bash
    node app.js
    ```

4. **Visit the application:**
    Open your browser and go to:
    ```
    http://localhost:8080
    ```

## Usage

1. When you first visit the app, you'll be redirected to the `/posts` page where all posts are displayed.
2. You can create a new post by clicking on the "New Post" button, filling out the form, and submitting it.
3. Click on a post to view its details.
4. Edit or delete posts directly from the post detail page.

## Routes

- **GET /**: Redirects to `/posts`
- **GET /posts**: Displays all posts
- **GET /posts/new**: Displays the form to create a new post
- **POST /posts**: Handles creating a new post
- **GET /posts/:id**: Displays details of a specific post
- **GET /posts/:id/edit**: Displays the form to edit a post
- **PATCH /posts/:id**: Handles updating an existing post
- **DELETE /posts/:id**: Handles deleting a post

## Technologies
- **Node.js**: Backend JavaScript runtime
- **Express.js**: Web framework for Node.js
- **EJS**: Embedded JavaScript templates for dynamic HTML
- **UUID**: Library to generate unique post IDs
- **Method-Override**: Allows support for PUT and DELETE methods in forms
- **CSS/Static files**: Public assets for styling

## Project Structure
```
|-- views/              # EJS templates for the app
|   |-- index.ejs       # List of all posts
|   |-- new.ejs         # Form to create a new post
|   |-- show.ejs        # Post detail page
|   |-- edit.ejs        # Edit form for a post
|-- public/             # Public folder for static files (CSS, images, etc.)
|-- app.js              # Main application file
|-- package.json        # Project dependencies and scripts
```
