# Firebase Guestbook

A lightweight, real-time guestbook web application built with HTML, CSS, JavaScript, and Firebase Realtime Database. Visitors can enter their name and a message, submit their entry, and see guestbook entries appear dynamically.

**Author:** Harsh Pandav

## ✨ Features

- **Simple message submission:** Enter a name and message through a minimal interface.
- **Real-time updates:** Listen for new entries using Firebase Realtime Database.
- **Persistent storage:** Store guestbook entries in the Firebase database.
- **Dynamic rendering:** Display new messages without manually refreshing the page.
- **Lightweight frontend:** Built with standard HTML, CSS, and JavaScript.

## 🛠️ Tech Stack

- HTML5
- CSS3
- JavaScript
- Firebase Realtime Database
- Firebase JavaScript SDK

## 📁 Project Structure

```text
firebase-guestbook/
├── index.html
├── style.css
└── script.js
```

## 🚀 Getting Started

### Prerequisites

- A Google account
- A Firebase project
- Firebase Realtime Database enabled
- A modern web browser
- A local web server for serving the application

### 1. Clone the repository

```bash
git clone https://github.com/Harshp110/firebase-guestbook-custom-harsh.git
cd firebase-guestbook
```

Adjust the repository URL and directory name if your GitHub repository uses a different name.

### 2. Configure Firebase

1. Open the [Firebase Console](https://console.firebase.google.com/).
2. Create a Firebase project or select an existing one.
3. Register a web application in the project.
4. Enable Realtime Database.
5. Copy the Firebase configuration for your web application.
6. Replace the placeholder values in `script.js` with your project's configuration.

The application currently contains placeholder values such as `YOUR_API_KEY` and `YOUR_PROJECT_ID`. It will not connect successfully until you configure them.

### 3. Configure database access

Configure Firebase Realtime Database Security Rules before using the application publicly.

The current code does not implement authentication, spam prevention, or server-side validation. Do not expose a publicly writable database without appropriate safeguards.

### 4. Run the application

Serve the project directory using a local development server, such as the VS Code Live Server extension, and open `index.html` through that server.

## ⚙️ How It Works

1. The visitor enters a name and message.
2. The `addEntry()` function reads the form values.
3. The application writes the entry to the `entries` path in Firebase Realtime Database.
4. After submission, the input fields are cleared.
5. A `child_added` listener receives existing and newly added entries and displays them in the guestbook.

Each entry is stored with two fields:

- `name` — the visitor's name.
- `msg` — the submitted message.

## 🔮 Potential Improvements

- Add input validation and message-length limits.
- Add Firebase Authentication or another appropriate abuse-prevention mechanism.
- Improve the responsive layout and accessibility.
- Display submission errors and loading states.
- Add timestamps to entries.
- Add moderation and spam protection.
- Migrate to the modular Firebase JavaScript SDK.
- Add automated tests and deployment instructions.

## 👨‍💻 Author

**Harsh Pandav**

- GitHub: [@Harshp110](https://github.com/Harshp110)

## 📄 License

No license is currently specified. Add a license file if you intend to define how others may use, modify, and distribute this project.
