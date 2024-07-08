# Music Player with Synchronized Lyrics Display

## Functional Requirements

### 1. Song Management

- **Upload Song**
  - Form to upload song files (MP3).
  - Store song file path and metadata in SQLite database.
- **Browse Songs**
  - List songs with metadata.
  - Search functionality based on title, artist, or album.
- **Play Song**
  - Retrieve song file and metadata from database.
  - Play song using HTML5 audio element.

### 2. Lyrics Management

- **Upload Lyrics**
  - Form to upload lyrics file (LRC format).
  - Store lyrics content and associated song ID in SQLite database.
- **Display Lyrics**
  - Fetch lyrics based on the song being played.
  - Display synchronized lyrics during playback.

### 3. Music Playback

- **Playback Controls**
  - Play, pause, stop, and seek functionalities.
  - Volume control.
- **Synchronized Lyrics**
  - Parse LRC file to get time-stamped lyrics.
  - Display the current lyric based on audio time updates.

### 4. Database Management

- **Database Schema**
  - Songs table: id, title, artist, album, file_path.
  - Lyrics table: id, song_id, content.
- **CRUD Operations**
  - Create, read, update, and delete songs and lyrics.
  - Retrieve songs and lyrics for playback.

## Required Features

### User Interface

- Intuitive UI for managing songs and lyrics.
- Responsive design to work on various devices.

### Performance

- Efficient audio playback without lags.
- Fast database queries to retrieve songs and lyrics.

### Security

- Safe storage of uploaded songs and lyrics.

### Usability

- Easy navigation and user-friendly design.
- Smooth synchronization of lyrics with song playback.

## Technological Stack

### Frontend

- **Next.js**: Server-side rendering and routing.
- **React**: Building UI components.
- **TypeScript**: Type-safe JavaScript.
- **Styled-components**: Styling.

### Backend

- **Node.js**: Server-side scripting.
- **better-sqlite3**: SQLite database management.

### Database

- **SQLite**: Lightweight and efficient local storage.

### Development Tools

- **ESLint**: Code quality.
- **Prettier**: Code formatting.
- **Jest**: Testing.

## Components and Modules

### Database Module

- better-sqlite3 setup and configuration.
- Tables for songs and lyrics.
- Queries for CRUD operations on songs and lyrics.

### Audio Player Component

- HTML5 audio element for playback.
- Controls for play, pause, and seek.
- Event listeners for time updates.

### Lyrics Synchronization Module

- Parser for LRC files.
- Functionality to display current lyric based on audio time.

### Upload and Management Interfaces

- Forms for uploading songs and lyrics.
- Interfaces for managing uploaded content.

## Conclusion

This document outlines the functional requirements and the necessary technological stack for creating a music player with synchronized lyrics display using Next.js, TypeScript, and better-sqlite3. The project will include song and lyrics management and a synchronized audio playback system, ensuring a robust and user-friendly application.
