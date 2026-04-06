# Book Tracker Frontend

## Overview

This is the frontend for the Book Tracker application. It is a simple website built using HTML, CSS, and JavaScript. The purpose of this project is to allow users to view, add, and update book data using a backend API.

## Table of Contents

* Overview
* Installation
* Usage
* API Integration
* Contributing
* License

## Installation & Setup

To run this project locally:

```bash
git clone https://github.com/hayezp/web.git
cd web
```

Then open `index.html` using Live Server in VS Code.

## Usage

Users can:

* View all books
* Add new books
* Update existing books

Navigation is available on every page.

Example screenshot:

<img src="images/screenshot.png" width="500">

## API Integration

The frontend connects to the backend API using fetch requests.

Example:

```javascript
fetch("https://module5-backend-api.onrender.com/api/v1/books")
```

## Contributing

To contribute:

1. Fork the repository
2. Create a new branch
3. Make changes
4. Submit a pull request

## License

This project is licensed under the MIT License.