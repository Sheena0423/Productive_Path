### **Project Title:**  
**Productive Path**

### **Project Overview:**  
*Productive Path* is a full-stack application designed for managing categories and products efficiently. The project focuses on basic CRUD operations for both categories and products, with server-side pagination to enhance data management. The relation between categories and products follows a one-to-many mapping, where each category can have multiple products. The system also integrates category details when retrieving individual product information.

### **Key Features:**
1. **Category Management:** CRUD operations for categories.
2. **Product Management:** CRUD operations for products.
3. **Pagination:** Server-side pagination for retrieving categories and products.
4. **One-to-Many Relationship:** A category can have multiple associated products.
5. **REST APIs:** Well-defined APIs for accessing and managing categories and products.

### **Technologies and Framework Used:**
- **Backend:** Spring Boot (for application setup), JPA, Hibernate (for ORM), REST controllers.
- **Database:** Relational Database (RDB) configuration, using annotations for configuration.
- **Others:** Maven (for dependency management), and server-side pagination for efficient data fetching.

### **Setup and Installation:**
1. Clone the repository:  
   ```
   git clone https://github.com/Sheena0423/Productive_Path.git
   ```
2. Open the project in your preferred IDE (IntelliJ, Eclipse, etc.).
3. Configure your database in the application.properties file.
4. Run the Spring Boot application using:  
   ```
   mvn spring-boot:run
   ```

### **Usage and Information:**

Below are the available APIs for both **Category** and **Product** management:

#### **Category CRUD APIs:**

1. **Get all categories:**  
   `GET /api/categories?page={page_number}`  
   Example:  
   ```
   http://localhost:8080/api/categories?page=3
   ```

2. **Create a new category:**  
   `POST /api/categories`

3. **Get category by Id:**  
   `GET /api/categories/{id}`  
   Example:  
   ```
   http://localhost:8080/api/categories/{id}
   ```

4. **Update category by Id:**  
   `PUT /api/categories/{id}`

5. **Delete category by Id:**  
   `DELETE /api/categories/{id}`

#### **Product CRUD APIs:**

1. **Get all products:**  
   `GET /api/products?page={page_number}`  
   Example:  
   ```
   http://localhost:8080/api/products?page=2
   ```

2. **Create a new product:**  
   `POST /api/products`

3. **Get product by Id:**  
   `GET /api/products/{id}`

4. **Update product by Id:**  
   `PUT /api/products/{id}`

5. **Delete product by Id:**  
   `DELETE /api/products/{id}`

---
