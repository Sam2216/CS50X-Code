# CS50X-Code
The code of the project CS50X

# Note-Taking Web Application

#### Video Demo: [https://www.youtube.com/watch?v=DDV1K2mT4Ec]

## Description:
This project is a web-based note-taking application built using the Flask web framework and SQLAlchemy for database management. The application allows users to create, view, update, and delete notes. Each note consists of a title, content, and a timestamp indicating when it was created.

## Files:
- `app.py`: This Python script contains the main application code. It defines the Flask routes, database model, and view functions. The code handles HTTP requests and interactions with the database.
- `templates/`: This folder contains HTML templates used to render the web pages:
  - `index.html`: Displays a list of all notes with their titles and creation dates.
  - `new_note.html`: Provides a form for users to create a new note. Users can enter a title and content for the note.
  - `view_note.html`: Shows the details of a specific note, including its title, content, and creation date.
  - `update_note.html`: Allows users to edit and update a note's title and content.
- `notes.db`: This SQLite database file stores note data. It includes tables for notes, each with columns for the note's ID, title, content, and creation date.

## Design Choices:
- **SQLite Database**: We chose SQLite for its simplicity and portability. It's well-suited for small to medium-sized applications like this one. For larger projects, other databases like PostgreSQL or MySQL might be more appropriate.
- **Flask Web Framework**: Flask was selected due to its lightweight nature, making it ideal for rapid development of web applications. It provides the necessary tools for routing, handling requests, and rendering templates.
- **HTML Templates**: HTML templates are used to separate the presentation layer from the application logic. This separation enhances maintainability and allows for easy customization of the user interface.
- **Secret Key**: The secret key is set to 'secret_key' for session security. In a production environment, this key should be kept secret and more securely managed.

## How to Run:
1. Clone this repository to your local machine.
2. Install the required dependencies using `pip install Flask Flask-SQLAlchemy`.
3. Navigate to the project directory.
4. Run the application with `python app.py`.
5. Access the application in your web browser at `http://localhost:5000`.

## Usage:
- Visit the home page (`http://localhost:5000`) to view a list of existing notes.
- Click the "New Note" button to create a new note with a title and content.
- Click on a note title to view its details, including the content and creation date.
- On the note detail page, you can also edit the note's title and content by clicking the "Edit" button.
- To delete a note, click the "Delete" button on the note detail page.

submit50

