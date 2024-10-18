# Snippet Box

**Snippet Box** is a web application that lets people paste and share snippets of text — similar to services like Pastebin or GitHub’s Gists. This project is built step-by-step following Alex Edwards' "Let's Go" book.

## Project Overview

The **Snippet Box** application starts simple, with just one web page for viewing and submitting snippets. As we progress, the application evolves with more advanced features, including routing, database integration, and user authentication. By the end of the book, the application will include:

- Ability to create and share text snippets.
- View snippets through unique URLs.
- User registration and authentication.
- Restricting access to snippet creation for registered users.
- HTTPS configuration for secure communication.
- Session management and middleware implementation.

## Features

- **Text Snippets**: Create and share snippets of text with expiration options.
- **User Authentication**: Registered users can log in and manage their own snippets.
- **HTTPS**: Secure communications using TLS encryption.
- **Session Management**: Cookie-based sessions to handle user login and persistence.

## Project Structure

Here's the basic structure of the project:

```bash
├── cmd/                    # Main application entry point and handlers
│   ├── web/
│   │   ├── main.go         # Application entry point
│   │   └── handlers.go     # HTTP handlers for processing requests
│
├── pkg/                    # Package directory (for reusable logic and helpers)
│
├── ui/
│   ├── html/               # HTML templates for rendering views
│   └── static/             # Static assets (CSS, JavaScript, images)
