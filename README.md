# 🎬 Movie Search App

## 📌 Project Overview
The **Movie Search App** is a web application that allows users to search for movies and view detailed information such as title, release year, genre, director, and plot summary.

The application fetches movie data from the OMDb API and dynamically displays the results using JavaScript.

---

## 🚀 Features
- Search movies by title
- Display movie posters and release year
- View detailed movie information
- Responsive design for desktop and mobile
- Error handling for invalid searches

---

## 🛠 Technologies Used
- HTML
- CSS
- JavaScript (ES6)
- Fetch API
- REST API

---

## 💻 Example Code

### Fetch Movie Data from API

```javascript
const API_KEY = "YOUR_OMDB_API_KEY";

async function searchMovies(query) {
  const response = await fetch(`https://www.omdbapi.com/?s=${query}&apikey=${API_KEY}`);
  const data = await response.json();
  console.log(data);
}
