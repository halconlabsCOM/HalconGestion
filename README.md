# HalconPOS

**HalconPOS** is a robust and modern Point of Sale (POS) system built with **Java Swing** and **MySQL**, designed to streamline retail operations. It features a sleek user interface powered by **FlatLaf**, comprehensive inventory management, and dynamic reporting capabilities.

## 🚀 Key Features

### 🛒 Point of Sale (POS)
- **Fast Checkout**: Efficient sales processing with barcode scanning support.
- **Dynamic Cart**: Real-time calculation of totals, taxes, and change.
- **Payment Methods**: Support for Cash, Card, and other payment types.
- **Invoice Generation**: Automatic generation of sales receipts.

### 📦 Inventory Management
- **Product Tracking**: full CRUD operations for products, categories, and units.
- **Stock Adjustments**: Audit-logged inventory movements (IN/OUT).
- **Barcode Support**: Integration with barcode scanners for quick product lookup.
- **Low Stock Alerts**: Visual indicators for products running low.

### 📊 Reporting & Analytics
- **Sales Reports**: Daily, monthly, and custom range sales reports.
- **JasperReports**: Professional PDF export for sales and inventory data.
- **Dashboards**: Visual summary of key performance metrics (planned).

### 🛡️ Security & Administration
- **Role-Based Access**: Granular permissions for Administrators vs. Cashiers.
- **Audit Logs**: Detailed tracking of sensitive actions (stock changes, void sales).
- **Secure Login**: User authentication system.

## 🛠️ Technology Stack

- **Language**: Java 17
- **UI Framework**: Java Swing (FlatLaf Theme)
- **Database**: MySQL 8.0
- **Build Tool**: Apache Maven
- **Key Libraries**:
    - **HikariCP**: High-performance JDBC connection pooling.
    - **JasperReports**: Reporting engine.
    - **Lombok**: Boilerplate code reduction.
    - **SwingX**: Extended Swing components.
    - **Apache POI**: Excel import/export support.

## 📋 Prerequisites

Before running the application, ensure you have the following installed:

- **Java Development Kit (JDK) 17** or higher.
- **MySQL Server 8.0**.
- **Apache Maven** (for building the project).

## ⚙️ Installation & Setup

1.  **Clone the Repository**
    ```bash
    git clone https://github.com/your-username/HalconPOS.git
    cd HalconPOS
    ```

2.  **Database Setup**
    - Create a MySQL database named `halconpos` (or as configured).
    - Import the provided SQL script (located in `/SQL` or root) to create tables and stored procedures.
    - Update database credentials in `src/main/resources/config.properties` or `DBConnection.java`:
      ```properties
      db.url=jdbc:mysql://localhost:3306/halconpos
      db.user=root
      db.password=your_password
      ```

3.  **Build the Project**
    ```bash
    mvn clean install
    ```

4.  **Run the Application**
    ```bash
    java -jar target/HalconPOS-1.0-SNAPSHOT.jar
    ```

## 📸 Screenshots

*(Add screenshots of the Login Screen, Main Dashboard, and POS Interface here)*

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
