# URL Shortener

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [Prerequisites](#prerequisites)
4. [Installation](#installation)
5. [Configuration](#configuration)
6. [Usage](#usage)
7. [Project Structure](#project-structure)
8. [Contributing](#contributing)
9. [License](#license)

## Introduction
This URL shortener application allows users to shorten long URLs into short, easy-to-remember URLs. The application is built using Node.js and uses shortid to generate unique short URLs. The project follows the Model-View-Controller (MVC) design pattern to keep the code organized and maintainable.

## Features
- Shorten long URLs
- Redirect short URLs to their original URLs
- Store and manage URLs in a database

## Prerequisites
- Node.js installed on your machine
- MongoDB installed and running

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/url-shortener.git
    cd url-shortener
    ```

2. Install dependencies:
    ```bash
    npm install
    ```

3. Install shortid:
    ```bash
    npm install shortid
    ```

## Configuration
1. Create a `.env` file in the root directory and add the following configuration:
    ```env
    MONGODB_URI=mongodb://localhost:27017/urlshortener
    PORT=3000
    ```

2. Ensure MongoDB is running and accessible at the specified `MONGODB_URI`.

## Usage
1. Start the application:
    ```bash
    npm start
    ```

2. Visit [http://localhost:3000](http://localhost:3000) in your browser to access the URL shortener.

3. Shorten a URL:
    - Enter a long URL in the input field and click "Shorten".
    - The shortened URL will be displayed, which can be used to redirect to the original URL.

## Project Structure
url-shortener/
│
├── controllers/
│ ├── urlController.js
│
├── models/
│ ├── urlModel.js
│
├── routes/
│ ├── index.js
│
├── views/
│ ├── index.ejs
│
├── .env
├── app.js
├── package.json
└── README.md

### Explanation:
- `controllers/urlController.js`: Handles the logic for shortening URLs and redirecting short URLs to original URLs.
- `models/urlModel.js`: Interacts with MongoDB to store and retrieve URLs.
- `routes/index.js`: Defines the routes for the application.
- `views/index.ejs`: The main view for the application.
- `app.js`: The main entry point for the application.

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request.


