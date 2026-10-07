# Inkly — Blog Management Platform

Inkly is a responsive, single-page blog platform for discovering, reading, and managing articles. It is built with plain HTML, CSS, and JavaScript, so it runs directly in a browser without a build step or external API.

## Features

- Browse sample articles and open a full article reader
- Search by title, author, category, or article text
- Filter articles by category
- Create, edit, and delete articles from the management page
- Like and bookmark articles, and add comments
- Persist articles, likes, bookmarks, comments, and the selected theme in browser local storage
- Switch between light and dark themes
- Responsive layouts for desktop, tablet, and mobile screens
- Empty states for no matching articles, no posts, and no comments

## Technology

- HTML5
- CSS3, including responsive media queries
- Vanilla JavaScript
- Browser local storage for persistence

There is no external data source or API. The app starts with sample posts defined in `index.html`; changes are saved in the current browser's local storage.

## Run locally

1. Clone or download this repository.
2. Open `index.html` in a modern browser.

Alternatively, serve the folder with any static file server. No package installation or build command is required.

## Usage

- Use the search field and category selector to find articles.
- Select a card to read the full article, react to it, bookmark it, or comment.
- Open **Manage Posts** to create, edit, or delete articles.
- Use the theme control in the header to switch appearance.

## Challenges and solutions

- **Keeping content after a refresh without a backend:** posts, reactions, comments, and theme preference are saved in browser local storage.
- **Showing useful feedback when content is missing:** the interface has empty states for searches with no matches, an empty post list, and articles without comments. It also reports when a post is unavailable.
- **Rendering user-written content safely:** post text and displayed metadata are escaped before being inserted into the page.

## Notes

Data is stored only in the browser and is not synchronized between devices or users. Clearing the browser's local storage removes saved changes and restores the sample content.
