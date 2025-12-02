+++
title = 'Music Api'
date = 2025-11-30T20:41:41-05:00
draft = false
+++

# Music Management API

A comprehensive REST API for managing a music app and its data, built with Laravel framework.

## Features
 - Complete CRUD operations
 - Data validation and error handling
 - MySQL database with Eloquent ORM
 - Docker containerization
 - RESTful API design principles

## Technology Stack
 - **Backend**: Laravel 12.40.02, PHP 8.2
 - **Database**: MySQL 8.0
 - **Containerization**: Docker, Docker Compose
 - **Testing**: Postman

## API Endpoints

## Albums Management

| Method | Endpoint             | Description               |
|--------|----------------------|---------------------------|
| GET    | `/api/albums`        | Retrieve all albums       |
| GET    | `/api/albums/{id}`   | Retrieve specific album   |
| POST   | `/api/albums`        | Create new album          |
| PUT    | `/api/albums/{id}`   | Update album              |
| DELETE | `/api/albums/{id}`   | Delete album              |

### Example Usage

### Create a Album
```bash
curl -X POST http://localhost:8080/api/albums \ 
  -H "Content-Type: application/json" \
  -d '{
    "albumName": "The Beatles 1967-1970",
    "artistName": "The Beatles",
    "numOfSongs": 37
   }'
```

### Response

```json
{
  "success": true,
  "message": "Album created successfully"
  "data": {
    "id": 3,
    "albumName": "The Beatles 1967-1970",
    "artistName": "The Beatles",
    "numOfSongs": 37
  }
}
```

## Artists Management

| Method | Endpoint            | Description              |
| ------ | ------------------- | ------------------------ |
| GET    | `/api/artists`      | Retrieve all artists     |
| GET    | `/api/artists/{id}` | Retrieve specific artist |
| POST   | `/api/artists`      | Create new artist        |
| PUT    | `/api/artists/{id}` | Update artist            |
| DELETE | `/api/artists/{id}` | Delete artist            |

### Example Usage

```bash
curl -X POST http://localhost:8080/api/artists \
  -H "Content-Type: application/json" \
  -d '{
    "name": "Queen",
    "agency": "Queen Agency"
    "genre": "Rock"
  }'
```

### Response

```json
{
  "success": true,
  "message": "Artist created successfully",
  "data": {
    "id": 3,
    "name": "Queen",
    "agency": "Queen Agency",
    "genre": "Rock"
  }
}
```

## Audiobook Management

| Method | Endpoint               | Description                 |
| ------ | ---------------------- | --------------------------- |
| GET    | `/api/audiobooks`      | Retrieve all audiobooks     |
| GET    | `/api/audiobooks/{id}` | Retrieve specific audiobook |
| POST   | `/api/audiobooks`      | Create new audiobook        |
| PUT    | `/api/audiobooks/{id}` | Update audiobook            |
| DELETE | `/api/audiobooks/{id}` | Delete audiobook            |

### Example Usage

```bash
curl -X POST http://localhost:8080/api/audiobooks \
  -H "Content-Type: application/json" \
  -d '{
    "bookName": "The Hobbit",
    "writerName": "J.R.R. Tolkien",
    "readerName": "Mary Poppins"
  }'
```

### Response

```json
{
  "success": true,
  "message": "Audiobook created successfully",
  "data": {
    "id": 3,
    "bookName": "The Hobbit",
    "writerName": "J.R.R. Tolkien",
    "readerName": "Mary Poppins"
  }
}
```

## Employees Management

| Method | Endpoint              | Description                |
| ------ | --------------------- | -------------------------- |
| GET    | `/api/employees`      | Retrieve all employees     |
| GET    | `/api/employees/{id}` | Retrieve specific employee |
| POST   | `/api/employees`      | Create employee            |
| PUT    | `/api/employees/{id}` | Update employee            |
| DELETE | `/api/employees/{id}` | Delete employee            |

### Example Usage

```bash
curl -X POST http://localhost:8080/api/employees \
  -H "Content-Type: application/json" \
  -d '{
    "name": "Doug",
    "email": "Doug@gmail.com",
    "department": "IT"
    "password": "DougTheGuy"
  }'
```

### Response

```json
{
  "success": true,
  "message": "Employee created successfully",
  "data": {
    "id": 3,
    "name": "Doug",
    "email": "Doug@gmail.com",
    "department": "IT"
    "password": "DougTheGuy"
  }
}
```

## Live Events Management

| Method | Endpoint              | Description                |
| ------ | --------------------- | -------------------------- |
| GET    |`/api/live-events`     | Retrieve all live events   |
| GET    |`/api/live-events/{id}`| Retrieve specific event    |
| POST   |`/api/live-events`     | Create live event          |
| PUT    |`/api/live-events/{id}`| Update live event          |
| DELETE |`/api/live-events/{id}`| Delete live event          |

### Example Usage

```bash
curl -X POST http://localhost:8080/api/live-events \
  -H "Content-Type: application/json" \
  -d '{
    "venue": "Vegas Strip",
    "artist": "Little Big Town",
    "day": "Saturday"
   }'
```

### Response

```json
{
  "success": true,
  "message": "Live Event created successfully",
  "data": {
    "id": 3,
    "venue": "Vegas Strip",
    "artist": "Little Big Town",
    "day": "Saturday"
   }
}
```
## Playlists Management

| Method | Endpoint              | Description                |
| ------ | --------------------- | -------------------------- |
| GET    | `/api/playlists`      | Retrieve all playlists     |
| GET    | `/api/playlists/{id}` | Retrieve specific playlist |
| POST   | `/api/playlists`      | Create new playlist        |
| PUT    | `/api/playlists/{id}` | Update playlist            |
| DELETE | `/api/playlists/{id}` | Delete playlist            |

### Example Usage

```bash
curl -X POST http://localhost:8080/api/playlists \
  -H "Content-Type: application/json" \
  -d '{
    "usersName": "Paul",
    "playlistName": "Study Vibes",
    "genre": "Blues"
   }
```

### Response

```json
{
  "success": true,
  "message": "Playlist created successfully",
  "data": {
    "id": 3,
    "usersName": "Paul",
    "playlistName": "Study Vibes",
    "genre": "Blues"
   }
}
```

## Podcast Management

| Method | Endpoint              | Description                |
| ------ | --------------------- | -------------------------- |
| GET    | `/api/podcasts`       | Retrieve all podcasts      |
| GET    | `/api/podcasts/{id}`  | Retrieve specific podcast  |
| POST   | `/api/podcasts`       | Create new podcast         |
| PUT    | `/api/podcasts/{id}`  | Update podcast             |
| DELETE | `/api/podcasts/{id}`  | Delete podcast             |

### Example Usage

```bash
curl -X POST http://localhost:8080/api/podcasts \
  -H "Content-Type: application/json" \
  -d '{
    "name": "Reddit stories",
    "hostName": "Greg Wash",
    "totalTime": 75
   }
```

### Response

```json
{
  "success": true,
  "message": "Podcast created successfully",
  "data": {
    "id": 3
    "name": "Reddit stories",
    "hostName": "Greg Wash",
    "totalTime": 75
   }
}
```

## Top Artists Management

| Method | Endpoint              | Description                |
| ------ | --------------------- | -------------------------- |
| GET    | `/api/top-artists`    | Retrieve all top artists   |
| GET    |`/api/top-artists/{id}`| Retrieve  top artist       |
| POST   | `/api/top-artists`    | Create new top artist      |
| PUT    |`/api/top-artists/{id}`| Update top artist          |
| DELETE |`/api/top-artists/{id}`| Delete top artist          |

### Example Usage


```bash
curl -X POST http://localhost:8080/api/top-artists \
  -H "Content-Type: application/json" \
  -d '{
    "name": "Selena Gomez",
    "genre": "Pop",
    "artistRank": 6
   }
```

### Response

```json
{
  "success": true,
  "message": "Top artist created successfully",
  "data": {
    "id": 3
    "name": "Selena Gomez",
    "genre": "Pop",
    "artistRank": 6
   }
}
```

## Top Songs Management

| Method | Endpoint              | Description                |
| ------ | --------------------- | -------------------------- |
| GET    | `/api/top-songs`      | Retrieve all top songs     |
| GET    | `/api/top-songs/{id}` | Retrieve  top songs        |
| POST   | `/api/top-songs`      | Create new top songs       |
| PUT    | `/api/top-songs/{id}` | Update top songs           |
| DELETE | `/api/top-songs/{id}` | Delete top songs           |

### Example Usage

```bash
curl -X POST http://localhost:8080/api/top-songs \
  -H "Content-Type: application/json" \
  -d '{
    "name": "All of the lights",
    "artist": "Kanye West",
    "songRank": 14
   }
```

### Response

```json
 "success": true,
  "message": "Top song created successfully",
  "data": {
    "id": 3
    "name": "All of the lights",
    "artist": "Kanye West",
    "songRank": 14
   }
}
```

## User Management

| Method | Endpoint              | Description                |
| ------ | --------------------- | -------------------------- |
| GET    | `/api/users`          | Retrieve all users         |
| GET    | `/api/users/{id}`     | Retrieve  user             |
| POST   | `/api/users`          | Create new user            |
| PUT    | `/api/users/{id}`     | Update user                |
| DELETE | `/api/users/{id}`     | Delete user                |

### Example Usage

```bash
curl -X POST http://localhost:8080/api/users \
  -H "Content-Type: application/json" \
  -d '{
    "name": "Daryl",
    "email": "DarylDixon@gmail.com",
    "password": "ThewalkingDead"
   }
```

### Response

```json
 "success": true,
  "message": "User created successfully",
  "data": {
    "id": 3
    "name": "Daryl",
    "email": "DarylDixon@gmail.com",
    "password": "ThewalkingDead"
   }
}
```
