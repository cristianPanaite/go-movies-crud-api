# Movie Management API

This Go code represents a Movie Management API using Gorilla Mux.

## Table of Contents

- [Dependencies](#dependencies)
- [Movie Struct](#movie-struct)
- [Director Struct](#director-struct)
- [API Endpoints](#api-endpoints)
  - [GET /movies](#get-movies)
  - [GET /movies/{id}](#get-movie)
  - [POST /movies](#create-movie)
  - [PUT /movies/{id}](#update-movie)
  - [DELETE /movies/{id}](#delete-movie)
- [Main Function](#main-function)

## Dependencies

The following packages are imported for this API:

- `encoding/json`: For encoding and decoding JSON data
- `fmt`: For formatted I/O
- `log`: For logging
- `math/rand`: For generating random numbers
- `net/http`: For HTTP server and client functionality
- `strconv`: For string conversions
- `github.com/gorilla/mux`: For building HTTP routers

## Movie Struct

The `Movie` struct represents a movie object with the following properties:

- `ID` (string): Unique identifier for the movie
- `Isbn` (string): International Standard Book Number for the movie
- `Title` (string): Title of the movie
- `Director` (*Director): Pointer to a Director object representing the movie's director

## Director Struct

The `Director` struct represents a movie director with the following properties:

- `Firstname` (string): First name of the director
- `Lastname` (string): Last name of the director

## API Endpoints

### GET /movies

- Description: Retrieves all movies
- Method: `GET`
- Path: `/movies`

### GET /movies/{id}

- Description: Retrieves a movie by ID
- Method: `GET`
- Path: `/movies/{id}`

### POST /movies

- Description: Creates a new movie
- Method: `POST`
- Path: `/movies`

### PUT /movies/{id}

- Description: Updates a movie by ID
- Method: `PUT`
- Path: `/movies/{id}`

### DELETE /movies/{id}

- Description: Deletes a movie by ID
- Method: `DELETE`
- Path: `/movies/{id}`