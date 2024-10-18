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
Here's the content formatted as a Markdown README file:

# Setup and Installation

To get started with the **Snippet Box** project, follow these steps:

1. Clone the repository:
```
git clone https://github.com/giftade/snippetbox.git
```

2. Navigate to the project directory:
```bash
cd $HOME/code/snippetbox
```

3. Create the necessary directory structure:
```bash
rm main.go mkdir -p cmd/web pkg ui/html ui/static
```

4. Create placeholder files for the main application:
```bash
touch cmd/web/main.go touch cmd/web/handlers.go
```

5. Set up your MySQL database and configure the `config.json` file with the appropriate credentials.

6. Run the application:
```bash
go run ./cmd/web
```

## Technologies Used

* **Go (Golang)**: Backend server and business logic
* **MySQL**: Relational database for storing snippets and user information
* **HTML/CSS/JS**: For rendering web pages and front-end interactivity
* **TLS/HTTPS**: Secure communication using SSL certificates
* **Session Management**: Cookie-based sessions for user authentication

## Roadmap

The project is developed step-by-step in the following phases:

1. Basic web server with a single page for creating and viewing snippets
2. Routing and database integration to manage multiple snippets
3. User authentication and authorization, restricting snippet creation to registered users
4. HTTPS setup for secure communication