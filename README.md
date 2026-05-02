# 🏥 NexusHealth - Clinical Management System

A modern, full-featured clinical management system built with Spring Boot 3.2.0 and Java 21. Manage appointments, consultations, doctors, patients, and pharmacist operations efficiently.

[![Java](https://img.shields.io/badge/Java-21-orange)](https://www.oracle.com/java/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.2.0-brightgreen)](https://spring.io/projects/spring-boot)
[![SQLite](https://img.shields.io/badge/SQLite-3-blue)](https://www.sqlite.org/)
[![Thymeleaf](https://img.shields.io/badge/Thymeleaf-3.1.2-green)](https://www.thymeleaf.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow)](LICENSE)

---

## 📋 Features

- 👨‍⚕️ **Doctor Management** - Register and manage doctors, specializations, and schedules
- 👥 **Patient Management** - Patient profiles, medical history, and demographics
- 📅 **Appointment Booking** - Streamlined appointment scheduling and cancellation
- 💬 **Consultations** - Consultation records and documentation
- 💊 **Pharmacy Management** - Medication inventory and prescriptions
- 👔 **Role-Based Access** - Admin, Doctor, Patient, Pharmacist, Receptionist roles
- 🔐 **Secure Authentication** - Spring Security with encrypted password handling
- 📊 **Dashboard** - Role-specific dashboards with key metrics
- 💾 **SQLite Database** - Lightweight, embedded database with automatic schema initialization

---

## 🚀 Quick Start

### ⚙️ Prerequisites

- **Java**: Java 21 (LTS) or higher
- **Maven**: 3.9.15+ (included as Maven Wrapper)
- **Git**: For cloning and version control
- **VSCode** (optional): For IDE-based execution

---

## 🎯 How to Run

### Option 1: 🖥️ Command Line (Windows/macOS/Linux)

1. **Clone the repository**:
   ```bash
   git clone https://github.com/IT24102111/Hospital-Management.git
   cd Hospital-Management
   ```

2. **Run the application**:
   ```bash
   # Using Maven Wrapper (recommended)
   ./mvnw spring-boot:run
   
   # Or on Windows
   mvnw.cmd spring-boot:run
   ```

3. **Access the application**:
   Open your browser and go to: `http://localhost:8081`

### Option 2: 🛠️ IDE (VS Code / IntelliJ / Eclipse)

1. **Clone and open** the project in your IDE
2. **Run** `ClinicApplication.java` as a Spring Boot application
3. **Access** at `http://localhost:8081`

---

## 🖥️ Live Demo

🚀 **Live Demo**: [http://localhost:8081](http://localhost:8081) (after running locally)

---

## 🛠️ Technologies Used

- **Backend**: Java 21, Spring Boot 3.2.0
- **Frontend**: Thymeleaf, HTML5, CSS3, JavaScript
- **Database**: SQLite
- **Build Tool**: Maven
- **Security**: Spring Security
- **ORM**: Hibernate/JPA

---

## 📁 Project Structure

```
src/
├── main/
│   ├── java/com/NexusHelth/
│   │   ├── ClinicApplication.java
│   │   ├── config/
│   │   ├── controller/
│   │   ├── dto/
│   │   ├── model/
│   │   ├── service/
│   │   └── util/
│   └── resources/
│       ├── application.properties
│       ├── schema.sql
│       ├── static/
│       └── templates/
└── test/
    └── java/com/NexusHelth/
```

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 📞 Contact

For questions or support, please open an issue on GitHub.
- 🧹 **Format Code**: Right-click → Format Document (Alt+Shift+F)

---

## 📊 Build & Test

### Clean Build
```bash
.\mvnw clean install
```

### Compile Only
```bash
.\mvnw clean compile
```

### Run Tests
```bash
.\mvnw clean test
```

### Generate Project Reports
```bash
.\mvnw clean test-compile
```

---

## 🗄️ Database

- **Type**: SQLite (embedded, no external installation needed)
- **Location**: `clinic.db` in the project root
- **Auto-Init**: Schema initializes automatically on first run
- **Data**: Includes sample admin account and test data

### Access Database

1. Download **DB Browser for SQLite**: https://sqlitebrowser.org/
2. Open `clinic.db` file
3. Browse tables and data

---

## 📦 Project Structure

```
NexusHealth/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/NexusHelth/
│   │   │       ├── ClinicApplication.java      (Main entry point)
│   │   │       ├── config/                     (Spring config)
│   │   │       ├── controller/                 (REST/Web controllers)
│   │   │       ├── dto/                        (Data transfer objects)
│   │   │       ├── model/                      (JPA entities)
│   │   │       ├── service/                    (Business logic)
│   │   │       └── util/                       (Helper utilities)
│   │   └── resources/
│   │       ├── application.properties          (Server config)
│   │       ├── schema.sql                      (Database schema)
│   │       ├── static/                         (JS, CSS, images)
│   │       └── templates/                      (HTML/Thymeleaf)
│   └── test/                                   (Unit/Integration tests)
├── .mvn/                                       (Maven wrapper)
├── mvnw / mvnw.cmd                            (Maven wrapper scripts)
├── pom.xml                                     (Maven configuration)
└── README.md                                   (This file)
```

---

## ⚙️ Configuration

### Server Port

Edit `src/main/resources/application.properties`:
```properties
server.port=8081
```

### Database Path

Default: `clinic.db` in project root. To change:
```properties
spring.datasource.url=jdbc:sqlite:/path/to/your/clinic.db
```

### Enable Debug Logging

```properties
logging.level.root=INFO
logging.level.com.NexusHelth=DEBUG
```

---

## 🔐 Default Login

- **Username**: admin
- **Password**: (Set during first signup or check database)

---

## 🛠️ Tech Stack

| Component | Version | Details |
|-----------|---------|---------|
| **Java** | 25 | Latest LTS version |
| **Spring Boot** | 4.0.5 | Web framework |
| **Spring Security** | 7.0.4 | Authentication & authorization |
| **Thymeleaf** | 3.x | Template engine |
| **SQLite JDBC** | 3.44.0.0 | Database driver |
| **Tomcat** | 11.0.20 | Embedded servlet container |
| **Maven** | 3.9.15 | Build tool |

---

## 📖 Copy to Another Computer

See [PORTABILITY.md](PORTABILITY.md) for detailed instructions on transferring the application to another machine.

---

## 🐛 Troubleshooting

### Port Already in Use
If port 8081 is already in use:
```properties
# In application.properties, change to:
server.port=8082
```

### Maven Build Fails
```bash
# Clear Maven cache
.\mvnw clean

# Rebuild
.\mvnw clean install
```

### Database Lock Error
Delete the old `clinic.db` file and restart:
```bash
del clinic.db
.\mvnw spring-boot:run
```

### Java Version Mismatch
Ensure Java 25 is set:
```bash
# Check Java version
java -version

# Set JAVA_HOME to Java 25
$env:JAVA_HOME = 'C:\path\to\java25'
```

---

## 📝 Recent Updates

- ✅ **Upgraded to Java 25** - Latest LTS version for modern features and security
- ✅ **Spring Boot 4.0.5** - Latest stable release
- ✅ **CVE Vulnerability Scanned** - All dependencies verified for security
- ✅ **VSCode Integration Guide** - Complete setup and run instructions

---

## 📞 Support

For issues or questions:
1. Check the Troubleshooting section above
2. Review Spring Boot documentation: https://spring.io/projects/spring-boot
3. Check SQLite JDBC documentation: https://github.com/xerial/sqlite-jdbc

---

## 📄 License

This project is part of the Zibrij initiative.

---

## 👤 Author

- **GitHub**: [ShajahanImdaad53](https://github.com/ShajahanImdaad53)
- **Repository**: [ZibrijProject](https://github.com/ShajahanImdaad53/ZibrijProject)

---

**Happy Coding! 🚀**
