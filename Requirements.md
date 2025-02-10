# Note-Taking App Requirements

## Overview
This is a note-taking application built using **React Native Expo**. The app allows users to create, edit, delete, search, and upload images or voice notes for their notes. The backend is powered by **Supabase**.

## Features
- **Add Notes**: Users can create new notes with text, images, and voice input.
- **Edit Notes**: Users can modify existing notes.
- **Delete Notes**: Users can remove notes from the database.
- **Search Functionality**: Users can search for notes using keywords.
- **Image Upload**: Users can attach images to notes.
- **Voice Input**: Users can record and attach voice notes.
- **Data Storage**: Notes are stored securely using Supabase.

## Tech Stack
### Frontend
- **React Native Expo**
- **React Navigation** (for navigating between screens)
- **Expo Image Picker** (for image uploads)
- **React Native Voice** (for voice input)
- **Tailwind CSS** (for styling)
- **ShadCN** (for UI components)

### Backend
- **Supabase** (for database and authentication)
- **Storage Bucket** (for storing images and voice recordings)

## UI Design
- **Primary Color:** Light Yellow (`#FFF9C4`)
- **Secondary Color:** White (`#FFFFFF`)
- **Accent/Font Color:** Black (`#000000`)

## Folder Structure
```
project-root/
│── src/
│   ├── components/        # Reusable UI components
│   ├── screens/           # App screens (Home, AddNote, EditNote, etc.)
│   ├── navigation/        # Navigation configuration
│   ├── utils/             # Helper functions and utilities
│── assets/                # Images, icons, and other assets
│── App.js                 # Entry point
│── package.json           # Project dependencies
│── README.md              # Documentation
```

## API Endpoints (Supabase)
- **`/notes` (POST)** - Add a new note
- **`/notes/:id` (PUT)** - Update an existing note
- **`/notes/:id` (DELETE)** - Remove a note
- **`/notes/search?query=` (GET)** - Search for notes
- **`/upload/image` (POST)** - Upload images
- **`/upload/audio` (POST)** - Upload voice recordings

## Additional Notes
- **Authentication**: Users may log in to sync notes across devices.
- **Offline Mode**: Basic offline support for viewing saved notes.
- **Minimalistic UI**: Clean, distraction-free design following the 3-color scheme.

---
This document serves as a reference for the development and implementation of the Note-Taking app.

