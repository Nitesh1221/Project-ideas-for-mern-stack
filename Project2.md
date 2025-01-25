### **2. Task Tracker App (Todo List)**

#### **Objective**  
Create a dynamic task tracker application where users can add, edit, delete, and mark tasks as complete or incomplete. This project will teach you the fundamentals of state management and CRUD (Create, Read, Update, Delete) operations, laying a foundation for more advanced projects.

---

### **Technologies and Topics**  
1. **Frontend**:  
   - **React.js**: For building the UI and managing states.  
   - **JavaScript**: For interactivity and logic building.  
   - **HTML**: For structuring content.  
   - **CSS**: For styling (or TailwindCSS for faster, modern styling).

2. **Backend (Optional)**:  
   - **JSON Server**: A mock backend to save tasks.  
   - **Firebase Firestore**: A free and simple backend solution.

3. **Additional Tools**:  
   - **Local Storage**: Save tasks locally without a backend (simpler option).  
   - **React Hooks**: Learn `useState`, `useEffect`, and custom hooks.

---

### **Features to Include**  
1. **Add New Tasks**  
   - Users can add tasks with a title, description, and optional due date.

2. **Mark as Complete/Incomplete**  
   - A checkbox to mark tasks as done, with a visual indicator (e.g., strikethrough).

3. **Edit Tasks**  
   - Allow users to update the title, description, or due date.

4. **Delete Tasks**  
   - Option to delete tasks permanently.

5. **Filter Tasks**  
   - View tasks by status (completed, incomplete, or all).

6. **Responsive Design**  
   - Ensure it works on mobile, tablet, and desktop devices.

7. **Optional Features**:  
   - Dark/Light mode toggle.  
   - Drag-and-drop for reordering tasks.

---

### **Steps to Build**  

#### **Phase 1: Plan**  
1. Sketch the app design and workflow (e.g., add, edit, delete tasks).  
2. Identify the features to implement.  
3. Decide whether to use local storage or a backend.

---

#### **Phase 2: Development**  
1. **Setup**:  
   - Install **Node.js** and initialize a React project with `npx create-react-app task-tracker`.  
   - Install dependencies like TailwindCSS (optional).

2. **Build the UI**:  
   - Create components for `TaskInput`, `TaskList`, and `TaskItem`.  
   - Style them using CSS or TailwindCSS.  

3. **State Management**:  
   - Use React’s `useState` to manage tasks as an array.  
   - Example:  
     ```javascript
     const [tasks, setTasks] = useState([]);
     ```

4. **Implement CRUD Operations**:  
   - **Add**: Add a task to the `tasks` array.  
   - **Delete**: Remove a task by filtering the `tasks` array.  
   - **Edit**: Use an edit form to modify a task’s details.  
   - **Complete/Incomplete**: Toggle the task’s `completed` property.  

5. **Optional: Connect a Backend**  
   - Install and set up **JSON Server**:  
     ```bash
     npm install -g json-server
     json-server --watch db.json
     ```  
   - Fetch and save tasks to the mock backend using `fetch` or `axios`.  

---

#### **Phase 3: Testing and Deployment**  
1. Test the app thoroughly for bugs and responsiveness.  
2. Deploy to **Netlify** or **Vercel** for free hosting.  
3. Push the code to GitHub to showcase your work.

---

### **Free Resources**  

#### **React.js Basics**  
1. [React Official Docs](https://reactjs.org/docs/getting-started.html)  
2. [React Crash Course - Traversy Media (YouTube)](https://www.youtube.com/watch?v=w7ejDZ8SWv8)  

#### **Styling**  
1. [CSS Flexbox Guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)  
2. [TailwindCSS Docs](https://tailwindcss.com/docs)  

#### **State Management**  
1. [React useState Hook](https://reactjs.org/docs/hooks-state.html)  
2. [React useEffect Hook](https://reactjs.org/docs/hooks-effect.html)  

#### **Optional Backend**  
1. [JSON Server Tutorial - Net Ninja](https://www.youtube.com/watch?v=TRcd2F8_rhI)  
2. [Firebase Firestore Quickstart](https://firebase.google.com/docs/firestore/quickstart)  

---

### **Cost Estimation**  
1. **Hosting**: Free (Netlify or Vercel).  
2. **Backend**: Free (JSON Server or Firebase).  
3. **Total Cost**: ₹0  

---

### **Time Estimation**  
- Planning: 1-2 days  
- Development: 10-12 days  
- Testing and Debugging: 2-3 days  
- Deployment: 1 day  
- **Total**: ~3 weeks  

---

### **Learning Outcomes**  
1. Mastery of React components, props, and state management.  
2. Understanding of dynamic rendering and interactivity.  
3. Experience with CRUD operations and optional backend integration.  
4. A practical project to demonstrate to recruiters.

---

Let me know if you'd like to start working on this or move to the next project (**Quiz Application**). 😊
