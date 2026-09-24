# CineManage – Movie Management System

CineManage is a responsive movie management website for organizing and managing a personal movie catalog. Users can browse movies, search titles, filter by genre, sort results, mark favourites, view movie details, and add, edit, or delete movies.

## Features

- Responsive movie catalog interface
- Movie search with instant filtering
- Filter movies by genre
- Sort movies by:
  - Rating
  - Release year
  - Title
- All Movies and Favourites tabs
- Grid and list viewing modes
- Add new movies
- Edit existing movies
- Delete movies with confirmation
- Mark movies as favourites
- Movie details modal
- Streaming platform links
- Poster URL support
- Automatic cinematic poster fallback
- Form validation
- Toast notifications
- Welcome tour modal
- Reset seed movie data option
- Empty state when no movies match the filters

## Movie Information

Each movie can contain:

- Movie title
- Genre
- Language
- Release year
- Rating
- Duration
- Poster URL
- Description
- Streaming platform
- Streaming link
- Favourite status

## Technologies Used

### HTML5

HTML5 is used to create the structure of the website, including:

- Header and navigation area
- Search bar
- Movie catalog section
- Filter and sorting controls
- Add/edit movie form
- Movie details modal
- Delete confirmation modal
- Welcome modal
- Footer

### CSS3

CSS3 is used for:

- Website layout and styling
- Responsive design
- Movie cards
- Grid and list layouts
- Modals and popup windows
- Buttons, badges, and form controls
- Hover effects and animations
- Dark cinematic theme
- Mobile and desktop compatibility

### JavaScript

JavaScript provides the website functionality, including:

- Rendering movie cards dynamically
- Searching movies
- Filtering movies by genre
- Sorting movies
- Switching between grid and list views
- Adding movies
- Editing movies
- Deleting movies
- Managing favourite movies
- Opening and closing modals
- Updating statistics
- Validating forms
- Displaying toast notifications
- Managing movie details
- Resetting seed data

### SVG Icons

Inline SVG icons are used throughout the website for:

- Search
- Add movie
- Edit
- Delete
- Favourite
- Star ratings
- Streaming links
- Grid and list view buttons
- Navigation and interface actions

## Project Structure

```text
movie-management-system/
└── public/
    ├── index.html
    ├── style.css
    └── app.js
```
## in server.js (which helps us as a backend)

GET, POST, PUT, and DELETE are HTTP methods used by APIs to perform CRUD operations:

Method	Purpose	Example
GET	Retrieve movies	GET /api/movies
POST	Add a new movie	POST /api/movies
PUT	Update an existing movie	PUT /api/movies/mov-1
DELETE	Remove a movie	DELETE /api/movies/mov-1

## Data Storage

The movie data is managed by the JavaScript application in `app.js`.

Movies added through the website are stored in the browser's local storage using the `localStorage` API (built-in Web Storage API provided by the browser) . This allows the movie data to remain available after refreshing or reopening the website in the same browser.

The application stores information such as:

- Movie details
- Favourite status
- User-added movies
- Edited movie information
- Deleted movie changes

The initial movies are seed data loaded by the application. The **Reset Seed Data** button restores the original movie catalog.

> Note: Browser local storage is local to the current browser and device. It is not a shared online database. Clearing browser storage or using another browser may remove or hide the saved movie data.

## How to Run the Website

1. Open the project in Visual Studio Code.
2. Open `public/index.html`.
3. Start the website using Live Server.
4. Open the displayed local URL in a browser.

The website can also be opened directly in a browser, but Live Server is recommended during development.

## How to Use

### Search Movies

Enter a movie title in the search bar to instantly filter the catalog.

### Filter Movies

Use the genre dropdown to display movies from a specific genre.

### Sort Movies

Use the sorting dropdown to sort movies by rating, release year, or title.

### Add a Movie

1. Click **Add Movie**.
2. Enter the required movie details.
3. Optionally add a poster URL and streaming link.
4. Click **Save Movie**.

### Edit a Movie

1. Open a movie's details.
2. Click **Edit**.
3. Update the information.
4. Save the changes.

### Delete a Movie

1. Open the movie details.
2. Click **Delete**.
3. Confirm the deletion.

### Mark a Favourite

Use the favourite button to add or remove a movie from the favourites list.

## Purpose

This project demonstrates how to build a complete frontend movie management application using HTML5, CSS3, and JavaScript. It includes dynamic user interfaces, CRUD operations, filtering, sorting, browser-based data storage, modal components, and responsive design.
