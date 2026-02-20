# ✈️ Airline Reservation System 🎟️🎫

## 📖 Overview

**TravelZilla** is a comprehensive desktop application that simulates an online airline ticket reservation system. This project provides a complete solution for users to search, book flights, and manage their reservations with an intuitive graphical user interface.

---

## ✨ Key Features

### 👤 User Features

- **User Registration & Authentication**: Secure registration and login system for customers
- **Flight Search**: Advanced search functionality for both domestic and international flights
- **Dynamic Filtering**: Filter flights by source, destination, date, and flight type
- **Flight Booking**: Seamless booking experience with passenger details collection
- **Booking Management**: View and manage flight bookings and preferences
- **Passenger Information**: Collect and store passenger details (name, age, gender, nationality)

### 🔧 Admin Features

- **Flight Management**: Add, update, and manage flight information
- **Inventory Control**: Manage seat availability and pricing
- **Flight Database**: View all active flights in the system
- **Domestic & International Flights**: Separate management for different flight types

---

## 🛠️ Technology Stack

| Component      | Technology             |
| -------------- | ---------------------- |
| **Frontend**   | Java Swing/AWT (GUI)   |
| **Backend**    | Java                   |
| **Database**   | MySQL                  |
| **IDE**        | NetBeans               |
| **Build Tool** | Apache Ant (build.xml) |

---

## 📁 Project Structure

```bash
Airline-Reservation-System/
├── Main.java                 # Application entry point
├── Dashboard.java            # Main flight search interface
├── LoginScreen.java          # User login interface
├── RegisterScreen.java       # User registration interface
├── Booking_Details.java      # Booking management & details
├── AdminInUpVw.java          # Admin panel for flight management
├── DBConnection.java         # Database connectivity handler
├── SplashScreen.java         # Application splash screen
├── *.form                    # NetBeans GUI form files
├── build.xml                 # Ant build configuration
├── manifest.mf               # JAR manifest file
└── README.md                 # Project documentation
```

---

## 🗄️ Database Schema

### Tables Used

1. **customer** - Stores user account information
   - Customer_ID, Customer_Name, Username, Password, Gender, Age, Country, etc.

2. **domestic_flights** - Domestic flight inventory
   - Flight_ID, Airlines, Source, Destination, Price, No_of_Seats, Availability, flight_date, flight_time

3. **international_flights** - International flight inventory
   - Flight_ID, Airlines, Source, Destination, Price, No_of_Seats, Availability, flight_date, flight_time

---

## 🚀 Getting Started

### Prerequisites

- Java Development Kit (JDK) 8 or higher
- MySQL Server 5.7 or higher
- NetBeans IDE (recommended)
- MySQL JDBC Driver (mysql-connector-java)

### Installation Steps

1. **Clone the Repository**

   ```bash
   git clone https://github.com/your-username/Airline-Reservation-System.git
   cd Airline-Reservation-System
   ```

2. **Database Setup**
   - Create a MySQL database named `airlines`
   - Import the database schema and sample data
   - Update connection credentials in `DBConnection.java`:

      ```java
      DriverManager.getConnection("jdbc:mysql://localhost:3306/airlines", "root", "your_password");
     ```

3. **Open in NetBeans**
   - Open NetBeans IDE
   - Go to File → Open Project
   - Navigate to the project directory and open it

4. **Build the Project**
   - Right-click on the project → Clean and Build
   - Or use command line: `ant build`

5. **Run the Application**
   - Right-click on the project → Run
   - Or use command line: `java -cp . travelzilla.Main`

---

## 📋 Application Workflow

### User Journey

1. **Application Start** → Splash Screen
2. **Dashboard** → Select flight type (Domestic/International)
3. **Search** → Choose source, destination, and date
4. **View Results** → Browse available flights
5. **Select Flight** → Click on desired flight
6. **Login/Register** → Authenticate or create new account
7. **Booking Details** → Enter passenger information
8. **Confirmation** → Complete booking

### Admin Journey

1. **Login** → Access admin panel
2. **View Flights** → See all flights in the system
3. **Add Flight** → Insert new flight details
4. **Update Flight** → Modify existing flight information
5. **Manage Inventory** → Update seat availability and pricing

---

## 🔐 Security Features

- User authentication with username and password
- Unique customer ID generation
- Session management for logged-in users
- Database connection pooling and validation

---

## 📝 Class Descriptions

| Class               | Purpose                                  |
| ------------------- | ---------------------------------------- |
| **Main**            | Entry point; initializes Dashboard       |
| **Dashboard**       | Main UI for flight search and selection  |
| **LoginScreen**     | User authentication interface            |
| **RegisterScreen**  | New user registration form               |
| **Booking_Details** | Passenger details collection and booking |
| **AdminInUpVw**     | Admin interface for flight management    |
| **DBConnection**    | Manages MySQL database connections       |
| **SplashScreen**    | Welcome screen with loading animation    |

---

## 🎯 Project Highlights

- **Complete End-to-End Solution**: From flight search to booking confirmation
- **User-Friendly Interface**: Intuitive GUI designed with Java Swing
- **Admin Control Panel**: Full control over flight inventory
- **Scalable Architecture**: Database-driven design allows easy expansion
- **Educational Value**: Great project for learning Java GUI, JDBC, and MySQL

---

## 🐛 Known Issues & Future Enhancements

### Current Limitations

- Single-threaded database operations
- No payment gateway integration
- Limited error handling in some modules
- No email notification system

### Future Enhancements

- Payment gateway integration (Stripe, PayPal)
- Email confirmations for bookings
- Mobile application version
- Advanced reporting and analytics
- Real-time seat availability updates
- Multi-language support
- Cancellation and refund management

---

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 👥 Contributors

- [Omkar Kajarekar](https://github.com/omkarkajarekar)
- [Vivek J. Utture](https://github.com/vivekjutture)
- [Rutuja Pandharpatte](https://github.com/RutujaPandharpatte)

---

## 📄 License

This project is open source and available under the MIT License.
