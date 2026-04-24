# 🛒 Ecommerce API (Spring Boot)

## 📌 Project Overview
This project is a RESTful API built using Spring Boot that simulates an e-commerce backend system.  
It supports CRUD operations for products and uses in-memory data storage (no database).

---

## ⚙️ Setup Instructions

1. Clone or download the repository
2. Open in IntelliJ IDEA or VSCode
3. Run the main class:
   EcommerceApiApplication.java
4. Server runs at:
   http://localhost:8080

---

## 📡 API Endpoints

### 🔹 GET all products
GET /api/v1/products

### 🔹 GET product by ID
GET /api/v1/products/{id}

### 🔹 FILTER products
GET /api/v1/products/filter?filterType=category&filterValue=Electronics

### 🔹 CREATE product
POST /api/v1/products

Sample Body:
{
  "name": "Shoes",
  "description": "Running shoes",
  "price": 2000,
  "category": "Sports",
  "stockQuantity": 5
}

### 🔹 UPDATE product
PUT /api/v1/products/{id}

### 🔹 PATCH product
PATCH /api/v1/products/{id}

### 🔹 DELETE product
DELETE /api/v1/products/{id}

---

## ✅ Status Codes Used

- 200 OK → Successful GET/PUT/PATCH
- 201 Created → Successful POST
- 204 No Content → Successful DELETE
- 400 Bad Request → Invalid input
- 404 Not Found → Product not found

---

## ⚠️ Validation Rules

- Product name must be at least 2 characters
- Price must be greater than 0
- Category is required
- Stock must not be negative

---

## ⚠️ Limitations

- Uses in-memory storage (data resets when server restarts)
- No database integration

---

## 🧪 Testing

Use Postman or any API testing tool to:
- Create products
- Retrieve products
- Update and delete products
- Test invalid inputs

---

## 👨‍💻 Author
Villanueva Nicole B.
Omela Raizalyn
