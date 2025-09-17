Blog Web Application

Description:
This is a simple blog web application built using Node.js and Express.js. It allows users to create, view, edit, and delete blog posts directly from the browser. The application uses in-memory storage for posts (no database, so data resets on server restart), making it ideal for learning purposes or as a starting point for a more robust blog system. The frontend is rendered with EJS templating for dynamic content, styled with Bootstrap for responsive design, and includes custom CSS for additional tweaks.
Key features:

Create new blog posts with a title and content.
View a list of all posts on the home page.
Edit existing posts.
Delete posts.
Basic form handling for user input.


Technologies Used:
Node.js: Runtime environment for server-side JavaScript.
Express.js: Web framework for handling routes, requests, and responses.
EJS: Templating engine for rendering dynamic HTML views.
Body-Parser: Middleware for parsing form data from HTTP requests.
Bootstrap: CSS framework for responsive and styled UI components.
Custom CSS: Additional styling in public/styles.css for layout and appearance.


Project Structure:
index.js: The main server file that sets up Express, defines routes for CRUD operations, and handles post data.
views/: Contains EJS template files for rendering pages.

index.ejs: Home page template that displays the list of posts.
edit.ejs: Template for editing a specific post.
partials/: Folder for reusable components like header.ejs and footer.ejs.


public/: Static assets served by Express.

styles.css: Custom stylesheet for the application's look and feel.


node_modules/: Installed dependencies (not tracked in Git; generated via npm install).
package.json & package-lock.json: Define project metadata, dependencies, and scripts.
.gitignore: Specifies files/folders to ignore in Git (e.g., node_modules).


Prerequisites:
Node.js (version 14 or higher recommended) installed on your machine.
A web browser (e.g., Chrome, Firefox) to access the app.


Installation:
Clone the repository from GitHub:
git clone https://github.com/amirkiarash/Blog-Web-Application.git

Navigate to the project directory:
cd Blog-Web-Application

Install the required dependencies:
npm install


How to Run:
Start the server:
node index.js
(Alternatively, if you have Nodemon installed globally for auto-reloading: nodemon index.js.)


Open your web browser and navigate to:
http://localhost:3500


The home page will load, showing any existing posts (initially empty). You can now create, edit, or delete posts.

To create a post: Fill in the form at the bottom of the home page and submit.
To edit a post: Click the "Edit" link next to a post.
To delete a post: Click the "Delete" link next to a post.



Note: Posts are stored in memory, so restarting the server will clear all data. For persistence, consider adding a database like MongoDB in future enhancements.
Troubleshooting

If you encounter errors during npm install, ensure your Node.js version is compatible and try deleting package-lock.json before reinstalling.
Port conflict: If port 3500 is in use, change the port variable in index.js to another value (e.g., 3000).
For any issues, check the console logs in your terminal for error messages.

License
This project is licensed under the ISC License. See the package.json for details.
Author
Kiarash (GitHub: amirkiarash)
Feel free to fork this repository and contribute improvements! If you have questions, open an issue on GitHub.
