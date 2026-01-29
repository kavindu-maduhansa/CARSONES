# CARSONES

CARSONES is a web-based vehicle rental and reservation management system built with Java. It allows users to manage vehicles, users, reservations, and locations through a user-friendly interface.

## Features

- **User Management:** Add, edit, delete, and search registered users with details such as name, license number, email, and contact info.
- **Vehicle Management:** Add, edit, delete, and search vehicles; manage details such as category, model, brand, gear, color, seating, fuel, plate number, and daily rate.
- **Reservations:** Create, update, search, and list reservations, including reservation ID, user, vehicle, location, pickup date, return date, and amount.
- **Location Management:** Add, edit, delete, and search branch locations (district, street, contact number, etc).
- **Rate Calculation:** Retrieve daily vehicle rates dynamically via servlet endpoints.
- **Modern UI:** Integrated with Bootstrap for responsive and stylish pages.

## Technologies Used

- Java (Servlets, JSP)
- Apache Tomcat
- Bootstrap 5 (CDN)
- JSP Standard Tag Library (JSTL)
- [Your Database Here] (MySQL/PostgreSQL/etc.)

## Getting Started

### Prerequisites

- Java 8+ (JDK)
- Apache Tomcat 9
- Maven (if using for dependency management)
- A compatible database (MySQL recommended)

### Setup & Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/kavindu-maduhansa/CARSONES.git
   ```

2. **Configure the database:**
   - Create a new database for the application.
   - Update DB connection settings in your source code or external properties file.

3. **Build and Deploy:**
   - Import the project into your IDE (IntelliJ IDEA, Eclipse, etc.).
   - Build the project using Maven or your IDE's build system.
   - Deploy the generated WAR or the `/Carsons` directory to your Tomcat `webapps` folder.

4. **Configure Tomcat:**
   - Review and adjust any `context.xml` or `server.xml` files as necessary:
     - `context.xml` controls resource loading.
     - `server.xml` configures your Tomcat engine, web application context, and logging.
   - Optionally, set up Tomcat users/roles in `tomcat-users.xml` for accessing admin/manager apps.

5. **Run the server:**
   - Start Tomcat.
   - Access the system at: `http://localhost:8080/Carsons`

## Usage

- Use the navigation menu to manage Users, Vehicles, Reservations, and Locations.
- Search, add, update, or delete records using the provided forms and tables.
- Toast messages notify you of action success or errors.
- Use the API endpoint `/reservation/getRate?vehicleId=...` to fetch daily rates via AJAX or HTTP requests.

## Contribution

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch: `git checkout -b my-feature`
3. Make your changes and commit: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-feature`
5. Open a pull request.

## License

[Update this section with your license]

## Author

- [kavindu-maduhansa](https://github.com/kavindu-maduhansa)

---

_This README was generated based on project structure and code. Please add additional details as needed._
