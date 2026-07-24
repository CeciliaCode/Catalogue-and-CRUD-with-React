# Computer Products Catalogue and Inventory CRUD

A full-stack web application for managing a catalogue of computer products and performing basic inventory operations.

The project provides a responsive React interface connected to a REST API built with Node.js, Express, TypeScript, TypeORM, and MySQL. Users can browse products and perform CRUD operations to create, view, update, and remove catalogue items.

## Features

* Browse a catalogue of computer products
* View product information and current stock
* Add new products to the catalogue
* Edit existing product information
* Delete products
* Perform basic inventory and stock management
* Navigate between application views using React Router
* Display operation feedback through toast notifications
* Responsive interface styled with Bootstrap and Sass
* REST API communication through Axios

## Tech Stack

### Frontend

* React
* TypeScript
* React Router
* Axios
* React Bootstrap
* Bootstrap
* Sass
* GSAP
* Font Awesome
* React Helmet
* React Toastify

### Backend

* Node.js
* Express
* TypeScript
* TypeORM
* MySQL
* JSON Web Tokens
* CORS
* Body Parser

## Project Structure

```text
Catalogue-and-CRUD-with-React/
├── Backend/
│   ├── src/
│   ├── package.json
│   ├── package-lock.json
│   └── tsconfig.json
│
└── Frontend/
    ├── public/
    ├── src/
    ├── package.json
    ├── package-lock.json
    └── tsconfig.json
```

The project is divided into two independent applications:

* `Frontend`: React client responsible for the user interface.
* `Backend`: Express REST API responsible for business logic, database access, and data management.

## Prerequisites

Before running the project, make sure you have installed:

* Node.js
* npm
* MySQL
* Git

## Installation

Clone the repository:

```bash
git clone https://github.com/CeciliaCode/Catalogue-and-CRUD-with-React.git
```

Enter the project directory:

```bash
cd Catalogue-and-CRUD-with-React
```

## Backend Setup

Navigate to the backend directory:

```bash
cd Backend
```

Install the dependencies:

```bash
npm install
```

Configure the MySQL connection in the backend source code according to your local environment.

You will need to provide values such as:

```text
Database host
Database port
Database username
Database password
Database name
```

Make sure the required MySQL database exists before starting the server.

Run the backend:

```bash
npm start
```

The backend starts through `ts-node` using the following entry point:

```text
Backend/src/index.ts
```

## Frontend Setup

Open another terminal and navigate to the frontend directory:

```bash
cd Frontend
```

Install the dependencies:

```bash
npm install
```

Start the React development server:

```bash
npm start
```

Open the application in your browser:

```text
http://localhost:3000
```

The page automatically reloads when changes are made to the source code.

## CRUD Operations

The application follows the four fundamental CRUD operations:

| Operation | Description                                     |
| --------- | ----------------------------------------------- |
| Create    | Add a new computer product to the catalogue     |
| Read      | Retrieve and display product information        |
| Update    | Modify product details or inventory information |
| Delete    | Remove a product from the catalogue             |

## API Architecture

The frontend communicates with the Express backend through HTTP requests using Axios.

```text
React Client
     │
     │ HTTP requests
     ▼
Express REST API
     │
     │ TypeORM
     ▼
MySQL Database
```

This separation keeps the user interface, server-side logic, and data persistence organized into independent application layers.

## Available Scripts

### Backend

```bash
npm start
```

Runs the Express API using TypeScript and `ts-node`.

### Frontend

```bash
npm start
```

Runs the React application in development mode.

## Learning Objectives

This project demonstrates:

* Building a full-stack application with React and Node.js
* Developing RESTful API endpoints with Express
* Implementing CRUD operations
* Connecting a Node.js application to MySQL
* Using TypeORM for database access
* Consuming APIs from React with Axios
* Creating reusable React components
* Managing navigation with React Router
* Styling responsive interfaces with Bootstrap and Sass
* Structuring frontend and backend applications separately
