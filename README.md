## This project is a full-stack web application built with ReactJS for the frontend and Express with Sequelize for the backend. The application connects to a MySQL database and allows users to perform CRUD operations on blog posts.

## Backend (src/server)
The backend is built with Node.js, Express, and Sequelize. It connects to a MySQL database to handle CRUD operations for blog posts.
Endpoints
GET /posts: Fetch all posts
GET /posts/:id: Fetch a single post by ID
POST /posts: Create a new post
PUT /posts/:id: Update an existing post
DELETE /posts/:id: Delete a post by ID

## Create a Database and User
Log in to the MySQL server:

mysql -u root -p
Enter the root password you set during the MySQL installation.

## Create a new database:

CREATE DATABASE blog_db;
Create a new user and grant privileges:

CREATE USER 'blog_user'@'localhost' IDENTIFIED BY 'password';
GRANT ALL PRIVILEGES ON blog_db.* TO 'blog_user'@'localhost';
FLUSH PRIVILEGES;
Replace 'blog_user' with your desired username and 'password' with a strong password.

## Exit MySQL:

EXIT;

## Using Command Prompt
You can also start MySQL directly from the Command Prompt:

Open Command Prompt as Administrator:

Press Win + X and select Command Prompt (Admin) or Windows PowerShell (Admin).
Start the MySQL Service:
Type the following command and press Enter:
net start MySQL

If your MySQL service is named differently (e.g., MySQL80), use the appropriate name:
net start MySQL80

## Frontend (src/client)
The frontend is built with ReactJS and communicates with the backend API to display and manage blog posts.

