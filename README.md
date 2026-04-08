# EchoNotes (Real-Time Collaborative Notes) 📝✨

A modern, real-time collaborative note-taking app built with **SwiftUI** where multiple users can edit the same note simultaneously — just like Google Docs but native on iOS.


## [App Preview](screenshots/dashboard.png)

## ✨ Features

- **Real-time Multi-user Editing** — Multiple people can edit the same note at the same time with live updates
- **Live Sync** — Instant synchronization using Firebase Firestore listeners
- **Secure Authentication** — User sign-in with Firebase Authentication (Email/Google/Apple)
- **Low-Latency Collaboration** — WebSocket layer for smooth real-time text broadcasting
- **Smart Conflict Resolution** — Handles simultaneous edits gracefully with operational transformation / last-write-wins strategy
- **Clean & Beautiful UI** — Modern SwiftUI design with dark mode and smooth animations
- **Room-based Sharing** — Create or join collaborative rooms with shareable invite links

**Planned Features:**
- Rich text formatting (bold, italic, headings, lists)
- Image & file attachments
- Offline support with automatic sync on reconnect
- Version history
- Presence indicators (who is typing)

## 🛠 Tech Stack

- **SwiftUI** — Modern declarative UI framework
- **Firebase Firestore** — Real-time NoSQL database
- **Firebase Authentication** — Secure user management
- **WebSockets** — For ultra-low latency updates
- **MVVM + Repository Pattern** — Clean & scalable architecture
- **async/await & Swift Concurrency** — Modern asynchronous code
- **Combine** — For reactive data handling

## 📱 Screenshots

*(Add screenshots later in `/screenshots` folder)*

| Login | Note Editor | Live Collaboration | Room List |
|-------|-------------|--------------------|---------|
| ![Login](screenshots/login.png) | ![Editor](screenshots/editor.png) | ![Collab](screenshots/collaboration.png) | ![Rooms](screenshots/rooms.png) |

## 🏗 Architecture

- **MVVM Architecture** with Repository Pattern
- **Firestore Repository** for data operations
- **WebSocket Manager** for real-time broadcasting
- **Conflict-free Replicated Data Type (CRDT)** inspired logic for safe concurrent editing
- Full dependency injection for better testability

## 🚀 How to Run

1. Clone the repository
   ```bash
   git clone https://github.com/heygaurav1/Real-Time-Collaborative-Notes.git
