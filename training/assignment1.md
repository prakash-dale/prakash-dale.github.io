# Assignment 1

Crate a static html website

Following below instructions to crate the website.

#### **Part 1: Basic Website Without JavaScript**

1. **Install Prerequisites**
   - Ensure you have [Visual Studio Code](https://code.visualstudio.com/) installed.
   - Install the "Live Server" extension in VS Code for testing.

2. **Set Up the Project Structure**
   - Create a project folder, e.g., `StaticWebsite`.
   - Inside the folder, create the following files:
     - `index.html` (Home page)
     - `tr_detail.html` (Task Details page)
     - `styles.css` (CSS for styling)

3. **Create the Navbar**
   - Add a consistent navbar to both `index.html` and `tr_detail.html`.

   ```html
   <!-- Navbar Template -->
   <header>
       <nav>
           <a href="index.html">Home</a> |
           <a href="tr_detail.html">TR Detail</a>
       </nav>
   </header>
   ```

4. **Create the Home Page (`index.html`)**
   - Add a table to display tasks.

   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <link rel="stylesheet" href="styles.css">
       <title>Home</title>
   </head>
   <body>
       <header>
           <nav>
               <a href="index.html">Home</a> |
               <a href="tr_detail.html">TR Detail</a>
           </nav>
       </header>
       <main>
           <h1>Task List</h1>
           <table>
               <thead>
                   <tr>
                       <th>Task ID</th>
                       <th>Task Description</th>
                       <th>Assigned To</th>
                       <th>Due Date</th>
                   </tr>
               </thead>
               <tbody>
                   <tr>
                       <td>1</td>
                       <td>Fix Navbar</td>
                       <td>John Doe</td>
                       <td>2024-11-20</td>
                   </tr>
                   <tr>
                       <td>2</td>
                       <td>Update Table</td>
                       <td>Jane Smith</td>
                       <td>2024-11-25</td>
                   </tr>
               </tbody>
           </table>
       </main>
   </body>
   </html>
   ```

5. **Create the Task Detail Page (`tr_detail.html`)**
   - Display details of the first task in a form format.

   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <link rel="stylesheet" href="styles.css">
       <title>Task Detail</title>
   </head>
   <body>
       <header>
           <nav>
               <a href="index.html">Home</a> |
               <a href="tr_detail.html">TR Detail</a>
           </nav>
       </header>
       <main>
           <h1>Task Detail</h1>
           <form>
               <label for="taskId">Task ID:</label>
               <input type="text" id="taskId" value="1" readonly><br>
               <label for="description">Description:</label>
               <input type="text" id="description" value="Fix Navbar"><br>
               <label for="assignedTo">Assigned To:</label>
               <input type="text" id="assignedTo" value="John Doe"><br>
               <label for="dueDate">Due Date:</label>
               <input type="date" id="dueDate" value="2024-11-20"><br>
           </form>
       </main>
   </body>
   </html>
   ```

6. **Style the Website (`styles.css`)**
   - Add basic styling to enhance readability.

   ```css
   body {
       font-family: Arial, sans-serif;
       margin: 0;
       padding: 0;
   }
   header {
       background-color: #f4f4f4;
       padding: 10px;
       text-align: center;
   }
   nav a {
       margin: 0 10px;
       text-decoration: none;
       color: #333;
   }
   table {
       width: 80%;
       margin: 20px auto;
       border-collapse: collapse;
   }
   th, td {
       border: 1px solid #ddd;
       padding: 8px;
       text-align: left;
   }
   th {
       background-color: #f4f4f4;
   }
   main {
       padding: 20px;
   }
   form {
       width: 300px;
       margin: auto;
   }
   label {
       display: block;
       margin-top: 10px;
   }
   input {
       width: 100%;
       padding: 5px;
       margin-top: 5px;
   }
   ```

7. **Test the Website**
   - Open the project in VS Code.
   - Right-click on `index.html` and select **Open with Live Server** to test.

---

#### **Part 2: Update with Bootstrap**

1. **Include Bootstrap CSS**
   - Add the Bootstrap CDN link in the `<head>` section of both HTML files.

   ```html
   <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
   ```

2. **Update the Navbar**
   - Replace the plain navbar with a Bootstrap navbar.

   ```html
   <nav class="navbar navbar-expand-lg navbar-light bg-light">
       <a class="navbar-brand" href="#">Static Website</a>
       <div class="collapse navbar-collapse">
           <ul class="navbar-nav">
               <li class="nav-item">
                   <a class="nav-link" href="index.html">Home</a>
               </li>
               <li class="nav-item">
                   <a class="nav-link" href="tr_detail.html">TR Detail</a>
               </li>
           </ul>
       </div>
   </nav>
   ```

3. **Style the Table**
   - Add Bootstrap classes to the table in `index.html`.

   ```html
   <table class="table table-striped table-bordered">
   ```

4. **Style the Form**
   - Add Bootstrap classes to the form elements in `tr_detail.html`.

   ```html
   <form class="p-3 border rounded">
       <div class="form-group">
           <label for="taskId">Task ID:</label>
           <input type="text" class="form-control" id="taskId" value="1" readonly>
       </div>
       <div class="form-group">
           <label for="description">Description:</label>
           <input type="text" class="form-control" id="description" value="Fix Navbar">
       </div>
       <div class="form-group">
           <label for="assignedTo">Assigned To:</label>
           <input type="text" class="form-control" id="assignedTo" value="John Doe">
       </div>
       <div class="form-group">
           <label for="dueDate">Due Date:</label>
           <input type="date" class="form-control" id="dueDate" value="2024-11-20">
       </div>
   </form>
   ```

5. **Test the Updated Website**
   - Refresh the Live Server preview to see the Bootstrap-styled version of your site.

---

