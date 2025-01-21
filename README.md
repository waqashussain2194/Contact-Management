# Friends Manager

This project is a Ruby on Rails application for managing a list of friends. It allows users to ADD, VIEW, UPDATE and DELETE and organize friends' information dynamically. Every User can have their own contacts as well. The application uses Rails' built-in features for a smooth and responsive experience with Jquery.

## Features
- Add new friends dynamically.
- View a list of friends with their details.
- Organize and manage friends' information efficiently.
- Responsive UI for better usability.

---

## Setup Instructions

### Prerequisites
Ensure you have the following installed:
- Ruby (version specified in `.ruby-version` file)
- Rails (>= 7.0)
- SQLite3 (for the default database setup)
- Node.js (for managing JavaScript dependencies)
- Yarn (optional, for managing frontend assets)

### Steps

1. **Clone the Repository**:
    ```bash
        git clone <repository_url>
        cd friends

2. **Install Dependencies**:
    ```bash
        bundle install
        yarn install

3.  **Set Up the Database**:
    ```bash
        rails db:create
        rails db:migrate

4.  **SStart the Server**:
    ```bash
    rails server

Open your browser and navigate to http://localhost:3000.


**Design and Approach**

**Backend**:
   **FriendsController**:
      1:  Handles creating, updating, and listing friends.
      2:  Uses standard RESTful Rails actions to maintain simplicity and follow Rails conventions.

   **Models**:
      1:  Friend model manages validations and database interactions.

**Frontend**
    Rails Views:
      1:  Render dynamic content using Rails' built-in templating system.
    
    Bootstrap:
      1:  Provides a responsive design and consistent styling.

    JavaScript:
      1:  Rails' default JavaScript integration ensures smooth interactions and enhances user experience.


**Trade-offs and Design Decisions**
     
    SQLite3 for Development:
       
        Lightweight and sufficient for small-scale applications and local development.
        Can be swapped with PostgreSQL or another database for production.


    Bootstrap for Styling:

        Chosen for its simplicity and out-of-the-box responsive design capabilities.


    Rails Conventions:

        Leveraged Rails' conventions for faster development and better maintainability.

**Running Locally**

rails server

Open http://localhost:3000 in your browser to access the application.


**Future Improvements**

Add pagination for large datasets.
Implement user authentication and authorization.
Enhance UI with a modern frontend framework like React or Vue.js.
Deploy the application to a hosting platform (e.g., Heroku or Render).