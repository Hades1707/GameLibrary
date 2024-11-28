
# Game Management Web Application Report

---

## **Title and Cover Page**

**Title:** Game Management Web Application  
**Author:** David  
**Date:** [29/11/2024]

**Links:**  
- [Hosted Web Application](#)  
- [GitHub Repository](#)  




To run:
IN VSCODE CLI

node.js server.js

    http://localhost:5000/

---

## **Introduction**

The Game Management Web Application was developed to simplify the process of managing game-related data. This project addresses the increasing demand for digital platforms to handle game inventories, reviews, and pricing efficiently. Inspired by the dynamic growth of online game libraries and stores, this system was designed with scalability and security in mind to support future enhancements. 

The application offers a streamlined interface for creating, updating, and listing games. It caters to administrators and game enthusiasts who require a user-friendly solution for managing game information.

---

## **System Overview**

The system is a web-based application comprising both frontend and backend components, designed using modern development tools and frameworks. Below is a high-level overview of its structure:

### **Frontend**
- Built with React.js for dynamic user interfaces.
- CSS files (`App.css`, `style.css`, `index.css`) ensure a visually appealing and responsive design.
- Core frontend functionalities:
  - Adding new games via `AddGame.js`.
  - Listing games dynamically using `GameList.js`.
  - Updating game details through `UpdateGame.js`.

### **Backend**
- Developed with Node.js and Express.js, ensuring efficient server-side processing.
- Uses MongoDB as the primary database for scalability and document-based storage.
- Key backend components:
  - **Controllers:** Logic for handling game-related actions (e.g., creating and fetching games).
  - **Models:** Mongoose schema defining the structure of game data.
  - **Routes:** API endpoints for handling client requests.

### **Key Views and Interfaces**
- **Main Game Dashboard:** Displays the list of available games with filters and pagination.
- **Add/Edit Game Forms:** Intuitive forms for inputting or modifying game details.
- **Dynamic Filtering:** Allows users to search games by title.

### **System Architecture**
![System Architecture Diagram](#) *(Insert a visual representation of how frontend, backend, and database interact.)*

---

## **Key Design Decisions**

The following decisions were made to optimize performance and user experience:

1. **Frontend Technology:**
   - React.js was chosen for its component-based architecture and state management, enabling a seamless user experience.

2. **Backend Framework:**
   - Express.js was selected for its simplicity and robustness in handling API requests.

3. **Database Selection:**
   - MongoDB was used due to its flexibility in handling unstructured data and scalability for growing datasets.

4. **Pagination and Filtering:**
   - Implemented to ensure efficient data retrieval and user interaction, especially for large datasets.

---

## **Database Design**

The application utilizes a MongoDB database with a schema defined in `gameModel.js`. Below is a summary of its structure:

### **Entities and Relationships**
- **Game:** Central entity representing game data.
  - Fields include:
    - `title` (string, required)
    - `originalPrice` (string, default: "Free")
    - `discountedPrice` (string, default: "Free")
    - `description` (string, default: "No description available")
    - `recentReviewsSummary` and `allReviewsSummary` (strings, optional)

### **Entity Relationship Diagram**
*(Insert ER Diagram visualizing the schema.)*

### **Comparison: SQL vs. NoSQL**
- **NoSQL (MongoDB)** was chosen for its flexibility and ability to store nested data structures efficiently.
- SQL databases would require more rigid schemas, which might hinder future scalability.

---

## **Security and Scalability**

### **Security Measures**
1. **Input Validation:**
   - Controllers validate required fields to prevent incomplete data submissions.
2. **Environment Variables:**
   - Sensitive configurations like database credentials are stored securely in `.env` files.
3. **CORS:**
   - Ensures controlled access to the backend API from trusted sources.

### **Scalability Features**
1. **Pagination:**
   - Limits data sent to the client, reducing server load.
2. **Cloud Compatibility:**
   - MongoDB Atlas or similar services can be used to scale the database.
3. **Modular Codebase:**
   - Clean separation of concerns allows for easy extension and maintenance.

---

## **Conclusion and Reflection**

This project highlights the power of modern web technologies in solving practical problems. The Game Management Web Application provides a robust foundation for handling game data efficiently, with potential for additional features like user authentication and analytics.

### **Reflection**
Through this project, I enhanced my skills in full-stack development, focusing on React.js, Node.js, and MongoDB. Challenges included managing asynchronous operations and ensuring efficient database interactions, both of which were addressed with modular design and pagination. Future improvements could include:
- Adding user roles for enhanced access control.
- Integrating analytics for tracking game popularity.

---

## **Appendices**

- **Link to Hosted Application:** [Insert Link]  
- **Link to GitHub Repository:** [Insert Link]  

*(Ensure the screencast presentation is included in the final zip file submission.)*

---
