# MyInventory — Inventory Management System

MyInventory is a full-stack inventory management web application built with **React.js**, **Node.js**, **Express.js**, and **MySQL**. It provides account-based inventory management, a light/dark interface, and PDF export of inventory data.

## Features

- **User accounts:** Register and log in to a personal account.
- **Inventory management:** Add, view, edit, and delete inventory items.
- **Theme switching:** Toggle between light and dark modes.
- **PDF export:** Export inventory data as a PDF document.

## Technology Stack

| Area | Technologies |
| --- | --- |
| Frontend | React.js, JavaScript, Material UI, Emotion, Styled Components, Tailwind CSS |
| Backend | Node.js, Express.js |
| Database | MySQL |
| State management | Redux, Redux Thunk, Redux Persist |
| Authentication and sessions | JSON Web Tokens (JWT), cookies, Express sessions |
| API requests | Axios |
| PDF export | pdf-lib |
| Development and testing | npm, Nodemon, React Testing Library |

## Getting Started

### Prerequisites

- Node.js and npm
- MySQL

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/supeshasalya1/ERP-System.git
   cd ERP-System
   ```

2. Install the frontend and backend dependencies:

   ```bash
   cd client
   npm install
   cd ../server
   npm install
   ```

3. Create a `.env` file in the `server` directory and configure the database connection and other environment variables required by the application. **Do not commit your `.env` file or credentials.**

4. Start the backend from the `server` directory:

   ```bash
   npm start
   ```

5. In a separate terminal, start the frontend from the directory containing its `package.json` (typically `client`):

   ```bash
   cd client
   npm start
   ```

> **Setup note:** Check the actual project scripts and environment variable names before following these commands. The original project instructions specified starting the frontend from the repository root; use whichever directory contains the frontend's `package.json`.

## Development Team

MyInventory was **jointly designed and developed** by two co-developers who contributed collaboratively throughout the project. Responsibilities were shared across the development process rather than divided into separately owned modules.

| Developer | Role | GitHub |
| --- | --- | --- |
| **Kaween Wettewa** | Co-Developer | [@kaveenwettewa](https://github.com/kaveenwettewa) |
| **[@supeshasalya1](https://github.com/supeshasalya1)** | Co-Developer | [GitHub profile](https://github.com/supeshasalya1) |

### Note on Commit History

The application was developed collaboratively before the completed codebase was uploaded to GitHub in a single initial commit. As a result, the Git commit history does not fully represent each developer's work on the project.

## Contributing

Suggestions and improvements are welcome. You can open an issue or submit a pull request.
