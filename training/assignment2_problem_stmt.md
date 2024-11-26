# Assignment 2

## Convert static site to dynamic site.

### **Problem Statement: Dynamic Task Management Website**

**Context:**  
Convert static website created in Assignment 1 to dynamic site using plain javascript

**Requirements:**  
The website must have the following features:

1. **Home Page**  
   - Display a list of tasks in a table format.
   - The table should include the following columns:
     - Task ID
     - Task Description
     - Assigned To
     - Due Date
   - Data should not be hardcoded in the HTML but stored in a JavaScript object and dynamically rendered into the table.
   - The `Task ID` column should be clickable and function as a hyperlink.

2. **Task Detail Page**  
   - Clicking on a `Task ID` in the table should navigate to a **Task Detail Page**.
   - The page should show details of the selected task in a form with the following fields:
     - Task ID (read-only)
     - Task Description
     - Assigned To
     - Due Date
   - Task details should be populated dynamically based on the clicked `Task ID`. Pass the `Task ID` as a query string parameter and use JavaScript to retrieve the corresponding data.

3. **Additional Guidelines**
   - Use **plain HTML, CSS, and JavaScript** (no libraries or frameworks like React or Angular).
   - Organize your code into multiple files:
     - `index.html`: The home page.
     - `tr_detail.html`: The task detail page.
     - `data.js`: JavaScript file to store task data.
     - `script.js` and `detail.js`: JavaScript files to handle dynamic content on respective pages.
     - `styles.css`: CSS file for styling the website.
   - Use the **Live Server** extension in Visual Studio Code to test your solution.

**Example Data:**  
Use the following example tasks to populate the JavaScript object:

```javascript
const tasks = [
    { id: 1, description: "Fix Navbar", assignedTo: "John Doe", dueDate: "2024-11-20" },
    { id: 2, description: "Update Table", assignedTo: "Jane Smith", dueDate: "2024-11-25" },
    { id: 3, description: "Test Functionality", assignedTo: "Alice Brown", dueDate: "2024-11-30" },
];
```

**Deliverables:**  
1. A fully functional dynamic website that meets the requirements.
2. Clean and well-commented HTML, CSS, and JavaScript code.
3. Screenshots or a video demonstrating:
   - The task list displayed on the home page.
   - Navigation to the task detail page by clicking a `Task ID`.
   - Correct data being displayed in the detail page form.

**Evaluation Criteria:**  
- Correct implementation of dynamic table and form population using JavaScript.
- Code readability and maintainability.
- Proper navigation between pages and handling of query string parameters.
- Styling of the website for readability and usability.


