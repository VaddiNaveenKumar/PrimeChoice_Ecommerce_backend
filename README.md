
# 🛡️ PrimeChoice E-commerce Backend

This is the **backend service** for PrimeChoice, a secure, modular, and scalable e-commerce application.  
Built with **Java 17 + Spring Boot**, it features RESTful APIs, JWT authentication, role-based access, and robust data management using Spring Data JPA and MySQL.

## 🚀 Tech Stack

- **Language:** Java 17
- **Framework:** Spring Boot
- **Security:** Spring Security, JWT
- **Database:** MySQL (JPA/Hibernate)
- **Build & Dependency:** Maven

## 📁 Folder Structure

```plaintext
backend/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── example/
│   │   │           └── demo/
│   │   │               ├── admincontrollers/
│   │   │               ├── adminservices/
│   │   │               ├── controller/
│   │   │               ├── dto/
│   │   │               ├── entity/
│   │   │               ├── filter/
│   │   │               ├── repository/
│   │   │               └── service/
│   │   ├── resources/
│   │   │   └── application.properties
│   ├── test/java/
├── HELP.md
├── mvnw / mvnw.cmd
├── pom.xml
├── target/
```

## ✨ Features

- **JWT Authentication** for both user and admin
- **User Registration/Login**
- **Product Management:** CRUD (admin only)
- **Order Management:** Place/view orders
- **Role-based access:** Customer vs Admin endpoints
- **CORS enabled:** For integration with frontend
- **RESTful APIs:** Clean, testable routes

## 🔑 API Endpoints

- `POST /api/auth/register` – Register customer
- `POST /api/auth/login` – Login and get JWT
- `GET /api/products` – List all products
- `GET /api/products/{id}` – Product details
- `POST /api/admin/products` – Add product (admin)
- `PUT /api/admin/products/{id}` – Update product (admin)
- `DELETE /api/admin/products/{id}` – Remove product (admin)
- `POST /api/orders` – Place order (customer)
- `GET /api/orders` – List customer’s orders
- `GET /api/admin/orders` – View all orders (admin)

## ⚙️ Configuration

**Edit `src/main/resources/application.properties`:**

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/ecommerce_database
spring.datasource.username=YOUR_DB_USER
spring.datasource.password=YOUR_DB_PASSWORD
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
jwt.secret=YOUR_STRONG_SECRET
server.port=your_port_number
spring.web.cors.allowed-origin-patterns=your_frontend_hosting_port
```

## 🏃 How to Run Locally

1. Clone the repository:
    ```
    git clone https://github.com/VaddiNaveenKumar/PrimeChoice_Ecommerce_backend.git
    cd PrimeChoice_Ecommerce_backend
    ```
2. Configure application.properties (DB credentials, JWT secret).
3. Build and run:
    ```
    ./mvnw spring-boot:run
    ```
   or run via IDE.

## 🧪 Testing

- Test APIs via Postman or frontend app.
- Unit tests: `src/test/java/`

## 🔗 Integrations

- [Frontend Repository](https://github.com/VaddiNaveenKumar/PrimeChoice_Ecommerce_frontend)
- Deploy to Render.



## 👨💻 Author

Vaddi Naveen Kumar  
GitHub: [VaddiNaveenKumar](https://github.com/VaddiNaveenKumar)

**To make this a downloadable file, simply copy the above, paste into a new file, and save it as `README.md` in your backend’s root directory.**
