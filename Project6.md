### **6. E-Commerce Product Listing**

#### **Objective**  
Build a simplified e-commerce platform to showcase products, filter them based on categories, sort by price or rating, and add to a cart. This project introduces you to UI/UX best practices, state management, and basic e-commerce functionality.

---

### **Technologies and Topics**

1. **Frontend**:  
   - **React.js**: For building the user interface.  
   - **React Router**: For navigation between pages (Home, Product Details, Cart).  
   - **CSS/TailwindCSS**: For responsive styling.  
   - **Context API** or **Redux**: For state management (cart and filters).  

2. **Backend (Optional)**:  
   - **JSON Server**: For product data and cart management.  
   - **Firebase Firestore**: For a lightweight backend with real-time updates.

3. **Free Mock APIs**:  
   - **Fakestore API**: Free product data for testing.  
     [Fakestore API Documentation](https://fakestoreapi.com/)

---

### **Features to Include**

1. **Home Page**:  
   - Display all products in a grid layout with a thumbnail, name, price, and rating.  

2. **Filter and Sort**:  
   - Filter products by categories (e.g., electronics, clothing).  
   - Sort by price (low to high or high to low) or rating.  

3. **Product Details**:  
   - Display detailed product information on a separate page.  

4. **Add to Cart**:  
   - Allow users to add products to a cart and view the cart items.  

5. **Responsive Design**:  
   - Ensure the platform works on both desktop and mobile.  

6. **Optional Features**:  
   - Search bar for finding products.  
   - Pagination or infinite scroll for product lists.  
   - Checkout page for mock purchases.

---

### **Steps to Build**

#### **Phase 1: Plan**  
1. Define key pages:  
   - **Home**: Displays all products with filtering and sorting options.  
   - **Product Details**: Displays detailed info for a single product.  
   - **Cart**: Shows added products with a total price.  

2. Decide the product data structure.  

Example Product JSON:  
```json
[
  {
    "id": 1,
    "title": "Wireless Headphones",
    "price": 2999,
    "category": "Electronics",
    "rating": 4.5,
    "image": "https://example.com/headphones.jpg",
    "description": "High-quality wireless headphones with noise cancellation."
  }
]
```

---

#### **Phase 2: Development**

1. **Setup React Project**:  
   - Use `npx create-react-app ecommerce-platform`.  

2. **Add Routing with React Router**:  
   - Install React Router:  
     ```bash
     npm install react-router-dom
     ```  
   - Define routes for Home, Product Details, and Cart.  

Example Router Setup:  
```javascript
import { BrowserRouter as Router, Route, Routes } from "react-router-dom";

function App() {
  return (
    <Router>
      <Routes>
        <Route path="/" element={<Home />} />
        <Route path="/product/:id" element={<ProductDetails />} />
        <Route path="/cart" element={<Cart />} />
      </Routes>
    </Router>
  );
}
```

3. **Build Components**:  
   - `Home`: Displays the product list with filtering and sorting options.  
   - `ProductCard`: A reusable component for each product.  
   - `ProductDetails`: Displays details of a single product.  
   - `Cart`: Shows all added products with total price and quantity controls.  

4. **State Management**:  
   - Use `useContext` or `useReducer` for cart and filters.  
   - Example cart state:  
     ```javascript
     const [cart, setCart] = useState([]);
     
     const addToCart = (product) => {
       setCart([...cart, product]);
     };
     ```

5. **Filtering and Sorting**:  
   - Add a dropdown for sorting and checkboxes for category filtering.  
   - Use state to store the selected filters and apply them to the product list.

6. **Fetch Product Data**:  
   - Use the Fakestore API or mock product data.  
   - Fetch data with `useEffect`:  
     ```javascript
     useEffect(() => {
       fetch("https://fakestoreapi.com/products")
         .then((res) => res.json())
         .then((data) => setProducts(data));
     }, []);
     ```

7. **Optional Backend**:  
   - Use JSON Server or Firebase Firestore to store product and cart data.  

---

#### **Phase 3: Testing and Deployment**

1. Test for:  
   - Proper filtering and sorting functionality.  
   - Correct routing for product details and cart.  
   - Responsiveness on different devices.  

2. Deploy the app to **Netlify** or **Vercel**.  
3. Push the project to GitHub and showcase it in your portfolio.  

---

### **Free Resources**

#### **React and Routing**  
1. [React Router Official Docs](https://reactrouter.com/en/main)  
2. [React Component Docs](https://react.dev/learn)  

#### **Mock APIs**  
1. [Fakestore API](https://fakestoreapi.com/)  

#### **Frontend Styling**  
1. [TailwindCSS Docs](https://tailwindcss.com/docs)  
2. [CSS Grid Guide - MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout)  

#### **Backend**  
1. [JSON Server Setup](https://www.npmjs.com/package/json-server)  
2. [Firebase Firestore Quickstart](https://firebase.google.com/docs/firestore)  

---

### **Cost Estimation**

1. **Hosting**: Free (Netlify or Vercel).  
2. **Backend**: Free (JSON Server or Firebase).  
3. **Mock API**: Free (Fakestore API).  
4. **Total Cost**: ₹0  

---

### **Time Estimation**

- Planning: 1-2 days  
- Development: 14-18 days  
- Testing and Debugging: 2-3 days  
- Deployment: 1 day  
- **Total**: ~3-4 weeks  

---

### **Learning Outcomes**

1. Learn React Router for navigation and dynamic routes.  
2. Master state management with Context API or Redux.  
3. Understand fetching and displaying data from an external API.  
4. Gain experience in implementing filters, sorting, and a cart system.  
5. Develop responsive UI for real-world applications.  

---

Would you like to dive deeper into any feature or proceed to the next project (**Online Examination System**)? 😊
