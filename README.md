# alx-project-0x14
CineSeek is a modern movie discovery application built with Next.js, TypeScript, and Tailwind CSS. The application allows users to browse movies from the MoviesDatabase API, view movie details, and search for films by year or genre.

# CineSeek: Movie Discovery App

CineSeek is a modern movie discovery application built with Next.js, TypeScript, and Tailwind CSS. It integrates with the MoviesDatabase API to allow users to browse, search, and explore movie details by year or genre.

---

## API Overview

The MoviesDatabase API provides access to a vast collection of movie data, including titles, genres, release years, cast, crew, and trailers. It supports filtering, pagination, and detailed metadata for over 9 million titles and 11 million actors and crew members. The API is designed for fast, scalable movie discovery applications.

---

## Version

**API Version:** 1.0 (as listed on RapidAPI)

---

## Available Endpoints

- **GET /titles**  
  Fetches a list of movie titles with support for filtering by year, genre, and pagination.

- **GET /titles/search/title**  
  Searches for movies by title keyword.

- **GET /titles/{id}**  
  Retrieves detailed information about a specific movie by its ID.

- **GET /titles/random**  
  Returns a random movie title from the database.

- **GET /titles/{id}/crew**  
  Fetches crew and cast details for a specific movie.

- **GET /titles/{id}/trailers**  
  Retrieves trailer URLs for a specific movie.

---

## Request and Response Format

### Example Request

```http
GET /titles?year=2020&genre=Action&page=1
Host: moviesdatabase.p.rapidapi.com
Headers:
  X-RapidAPI-Key: YOUR_API_KEY
  X-RapidAPI-Host: moviesdatabase.p.rapidapi.com
