# Express.js: Note Taker

## Description

This assignment is to modify starter code to create an application called Note Taker that can be used to write and save notes. This application uses an Express.js back end and saves and retrieve note data from a JSON file.

The application’s front end has already been created. The assignment is to build the back end, connect the two, and then deploy the entire application to Heroku.

## User Story

A small business owner wants to be able to write and save notes
to organize thoughts and keep track of tasks to complete.

## Acceptance Criteria

When the user opens the Note Taker, the user is presented with a landing page with a link to a notes page.

When the user clicks on the link to the notes page, the user is presented with a page with existing notes listed in the left-hand column, plus empty fields to enter a new note title and the note’s text in the right-hand column.

When the user enters a new note title and the note’s text, a Save icon appears in the navigation at the top of the page.

When the user clicks on the Save icon, the new note the user has entered is saved and appears in the left-hand column with the other existing notes.

When the user clicks on an existing note in the list in the left-hand column, that note appears in the right-hand column.

When the user clicks on the Write icon in the navigation at the top of the page, the user is presented with empty fields to enter a new note title and the note’s text in the right-hand column.

## Mock-Up

The following images show the web application's appearance and functionality:

![Existing notes are listed in the left-hand column with empty fields on the right-hand side for the new note’s title and text.](./Assets/11-express-homework-demo-01.png)

![Note titled “Balance accounts” reads, “Balance account books by end of day Monday,” with other notes listed on the left.](./Assets/11-express-homework-demo-02.png)

## More Functionality

On the back end, the application includes a `db.json` file that is used to store and retrieve notes using the `fs` module.

The following HTML routes have been created:

* `GET /notes` returns the `notes.html` file.

* `GET *` returns the `index.html` file.

The following API routes has been created:

* `GET /api/notes` reads the `db.json` file and return all saved notes as JSON.

* `POST /api/notes` receives a new note to save on the request body, adds it to the `db.json` file, and then returns the new note to the client. Each note has a unique id when it's saved.

## Challenge Links

The URL of the functional, deployed to Heroku. https://dmk-note-taker.herokuapp.com/

The URL of the GitHub repository: https://github.com/dawn-kline-m/Note-Taker
