# resourcevau1t.ccbp.tech
---

# Resource Vault

**Resource Vault** is a dynamic, responsive web application designed to provide users with a collection of educational resources. It allows for the addition of new books and resources, and dynamically displays the available books through an API integration. The platform is built using **Node.js**, **Express.js**, **MongoDB**, and **HTML/CSS**.

## Features

- **Dynamic Book Listings**: Users can view a list of books stored in the database.
- **Add New Books**: Admin users can add new books via a form, which is saved to the MongoDB database.
- **Responsive Design**: The website is fully responsive and works on all devices, from mobile phones to desktops.
- **Interactive Search**: Users can search for specific books in the resources list.
- **API Integration**: Uses API calls to handle book data dynamically between front-end and back-end.
- **Open Source**: Free to use and contribute to.

## Tech Stack

- **Frontend**: HTML, CSS, JavaScript (for dynamic updates)
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **API**: RESTful API for interacting with the book data

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/AbhishekAdiga/resourcevau1t.ccbp.tech.git
cd resourcevau1t.ccbp.tech
```

### 2. Set Up Backend

Ensure that you have **Node.js** and **MongoDB** installed.

- Install backend dependencies:

```bash
cd server
npm install
```

- Create a `.env` file in the `server` directory and add the following configuration:

```env
DB_URI=mongodb://localhost:27017/resourcevault  # MongoDB connection URI
PORT=5000
```

- Start the backend server:

```bash
npm start
```

This will start the server on `http://localhost:5000`.

### 3. Set Up Frontend

- Navigate to the `client` directory and open the `index.html` file in your browser. You may want to configure your front-end to make AJAX requests to your local server (`http://localhost:5000`).

## API Endpoints

### POST /addBook

Adds a new book to the database.

**Request Body**:
```json
{
  "title": "Book Title",
  "author": "Book Author",
  "description": "Description of the book",
  "isbn": "123456789",
  "publishDate": "2024-01-01"
}
```

**Response**:
```json
{
  "title": "Book Title",
  "author": "Book Author",
  "description": "Description of the book",
  "isbn": "123456789",
  "publishDate": "2024-01-01"
}
```

### GET /books

Fetches a list of all books from the database.

**Response**:
```json
[
  {
    "title": "Book Title",
    "author": "Book Author",
    "description": "Description of the book",
    "isbn": "123456789",
    "publishDate": "2024-01-01"
  },
  {
    "title": "Another Book Title",
    "author": "Another Author",
    "description": "Another description",
    "isbn": "987654321",
    "publishDate": "2023-06-01"
  }
]
```

## Contributing

1. Fork the repository
2. Create a new branch (`git checkout -b feature-branch`)
3. Make your changes and commit them (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature-branch`)
5. Create a pull request

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgments

- [Node.js](https://nodejs.org/en/)
- [Express.js](https://expressjs.com/)
- [MongoDB](https://www.mongodb.com/)
- [Bootstrap](https://getbootstrap.com/)
- [Font Awesome](https://fontawesome.com/)

---

This **README.md** file provides clear instructions on how to set up and use the project, the tech stack, API documentation, and how others can contribute. You can update this further based on additional project requirements or specific deployment steps.
