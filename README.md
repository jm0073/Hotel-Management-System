https://livesql.oracle.com/apex/livesql/s/ca2ugqza017g3i6wuxtkx6q1c
# Hotel Management System

The **Hotel Management System** is an integrated platform designed to automate and streamline the operations of a hotel. It helps hotel managers and staff manage reservations, billing, room availability, staff assignments, and customer feedback, among other tasks.

## Project Overview

The primary goal of this project is to develop a software solution that simplifies the management of hotel operations by creating a centralized system for handling guests, employees, room inventory, and billing. This system also provides business intelligence insights to assist managers in decision-making.

## Features

### Client-Side
- **Room Reservation**: Allows customers to view room availability and book rooms in advance based on their preferences.
- **Guest Management**: Tracks guest information, including check-in and check-out records.
- **Billing and Payment**: Facilitates the generation of bills for guests, incorporating any additional services availed during their stay.
- **Feedback System**: Collects customer feedback to ensure service improvements.

### Admin-Side (Hotel Staff)
- **Employee Management**: Tracks staff assignments, work schedules, and performance.
- **Inventory Management**: Maintains records of hotel supplies and resources (e.g., toiletries, bedding).
- **Room Management**: Automates the process of assigning rooms to guests, as well as managing room maintenance.
- **Data Reporting**: Generates reports on guest statistics, room occupancy rates, revenue, and more.

## Database Structure

### Entities:
- **Hotel**: Stores hotel information.
- **Employee**: Contains employee details and job roles.
- **Inventory**: Manages the stock of items required for hotel operations.
- **Guest**: Stores guest details, including personal information and booking history.
- **Room**: Maintains records of room types, availability, and rates.
- **Bill**: Stores billing information for each guest, including services used.

### Relations:
- **Checked_in**: Tracks guests who have checked in.
- **Checked_out**: Tracks guests who have checked out.
- **Reserved**: Handles room reservation details.
- **Employs**: Connects employees to the hotel.
- **Keeps**: Tracks inventory management.
- **Has**: Tracks room details for each guest.
- **Pays**: Manages the payment process for guests.

### Normalization:
- The database follows 1NF, 2NF, and 3NF normalization to ensure efficient data storage and prevent redundancy.

### ER Diagram:
- An ER diagram has been created to illustrate the relationships between the entities within the system, simplifying the database structure.

## Technical Specifications

- **Backend**: PHP for server-side logic.
- **Frontend**: HTML, CSS, and JavaScript for the client-side interface.
- **Database**: MySQL for managing hotel data.
- **PL/SQL**: Procedures and functions were used for handling complex database operations.

## Setup Instructions

### Prerequisites
- **PHP**: Install PHP for server-side processing.
- **MySQL**: Install MySQL for database management.
- **Web Server**: Use XAMPP, WAMP, or another web server to run the application locally.

### Installation Steps
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/hotel-management-system.git
   cd hotel-management-system
   ```

2. **Database Setup**:
   - Import the provided SQL file into your MySQL database.
   - Example command:
     ```bash
     mysql -u root -p your_database_name < hotel_management.sql
     ```

3. **Configure the Database Connection**:
   - Update the `config.php` file with your database credentials:
     ```php
     $host = 'localhost';
     $db = 'hotel_db';
     $user = 'root';
     $password = 'your_password';
     ```

4. **Run the Application**:
   - Start your local web server (e.g., XAMPP or WAMP).
   - Access the project via:
     ```
     http://localhost/hotel-management-system/
     ```

## Usage

1. **User Functionality**:
   - Browse available rooms and make reservations.
   - View your reservation history and generate invoices for your stay.
   - Leave feedback on your experience.

2. **Admin Functionality**:
   - Add, update, or remove room listings.
   - Manage guest check-ins and check-outs.
   - Oversee hotel inventory and employee schedules.
   - Generate and view reports on hotel performance.

## Conclusion

The **Hotel Management System** ensures that guests can seamlessly book rooms and receive high-quality service, while hotel staff can manage operations effectively using a centralized system.

