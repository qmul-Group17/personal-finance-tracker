# 💰 Personal Finance Tracker 

**A sophisticated Java Swing-based personal finance management system with AI-powered Chinese context awareness, multi-user support, and intelligent transaction categorization.**

<div align="center">
  
![Java](https://img.shields.io/badge/Java-8+-blue?style=flat-square&logo=java)
![Swing](https://img.shields.io/badge/GUI-Swing-green?style=flat-square)
![AI](https://img.shields.io/badge/AI-Powered-purple?style=flat-square)
![Chinese](https://img.shields.io/badge/Context-Chinese-red?style=flat-square)

</div>

---

## ✨ Features

- **User Registration & Login**  
  - Secure login with SHA-256 hashed passwords  
  - All users stored in `users.json`

- **Per-User Transaction Files**  
  - Each user has a separate file: `transactions_<username>.json`

- **Manual Entry and Categorization**  
  - Add/edit/delete income or expense records
  - AI or keyword-based auto-categorization

- **CSV Import & Export**  
  - Import existing transactions from `.csv`
  - Export table data as `output.csv`

- **Chart Visualization**  
  - JFreeChart pie chart for income/expense distribution and line chart for trends
  - Budget expression with expenditure

- **AI Financial Analysis**
    - Chinese context-aware spending pattern analysis
    - Budget habit analysis with cultural insights
    - Shopping festival detection (Double 11, 618, Spring Festival)
    - Red packet transaction recognition
    - Personalized financial recommendations with seasonal context


---

### 📂 **Project Structure**
```
PersonalFinanceTracker/
├── 📁 bin/                        # Compiled classes
├── 📁 lib/                        # External dependencies
│   ├── gson-2.10.1.jar           # JSON processing
│   ├── jfreechart-1.5.3.jar      # Chart visualization
│   └── junit-platform-console-standalone-1.9.2.jar  # Testing
├── 📁 src/                        # Source code
│   ├── 📁 controller/             # Business logic
│   │   ├── AppConfig.java
│   │   ├── TransactionController.java
│   │   ├── UserController.java
│   │   ├── TransactionCategorizer.java
│   │   ├── MLTransactionCategorizer.java
│   │   └── CSVImporter.java
│   ├── 📁 model/                  # Data models
│   │   ├── Transaction.java
│   │   ├── User.java
│   │   └── Currency.java
│   ├── 📁 util/                   # Utilities
│   │   ├── HashUtil.java
│   │   └── JsonUtil.java
│   ├── 📁 view/                   # UI components
│   │   ├── MainFrame.java
│   │   ├── LoginFrame.java
│   │   ├── EditTransactionDialog.java
│   │   ├── TransactionDialog.java
│   │   └── APISettingsDialog.java
│   └── Main.java                  # Application entry point
├── 📁 test/                          # TDD Test Implementation
│   ├── 📁 controller/
│   │   ├── RedPacketDetectionTDDTest.java    # 🔴🟢🔵 TDD Example
│   │   └── TransactionCategorizerTest.java   # Transaction categorization tests
│   └── 📁 model/
│       └── UserTest.java     
└── 📁 PersonalFinanceTracker/     # User data storage
    ├── users.json                 # User registry
    └── transactions_<user>.json   # Individual user data
```


### 🔧 **Dependencies & Technologies**
| Technology | Version | Purpose |
|------------|---------|---------|
| ☕ **Java** | 8+ | Core application framework |
| 🎨 **Swing** | Built-in | GUI framework |
| 📊 **JFreeChart** | 1.5.3 | Advanced chart visualization |
| 🔗 **Gson** | 2.10.1 | JSON data serialization |
| 🧪 **JUnit** | 5 | Test-driven development |
| 🤖 **DeepSeek API** | Latest | AI-powered analysis |

---

## 🏆 Project Highlights

### 🎓 **Academic Excellence**
- **Test-Driven Development**: Comprehensive TDD implementation
- **Design Patterns**: MVC architecture with separation of concerns
- **Code Quality**: Well-documented, maintainable codebase
- **Cultural Awareness**: Chinese context integration

### 💡 **Innovation Features**
- **AI-Powered Categorization**: First-of-its-kind Chinese context awareness
- **Cultural Intelligence**: Shopping festival and red packet detection
- **Smart Analytics**: Behavioral pattern recognition
- **User Experience**: Intuitive interface with cultural considerations

### 🔬 **Technical Achievements**
- **Multi-User Architecture**: Scalable user management system
- **Data Integrity**: Robust error handling and validation
- **Performance Optimization**: Efficient data processing and visualization
- **Cross-Platform Compatibility**: Pure Java implementation

---

## ▶️ How to Compile & Run

### ⚡ **Installation & Setup**

1. **Download Dependencies**
   ```bash
   # Ensure all JAR files are in the lib/ directory
   lib/gson-2.10.1.jar
   lib/jfreechart-1.5.3.jar
   lib/junit-platform-console-standalone-1.9.2.jar
   ```

2. **Compilation**
   ```bash
   # Compile all source files
   javac -cp "lib/gson-2.10.1.jar;lib/jfreechart-1.5.3.jar" -d bin src/**/*.java
   ```

3. **Execution**
   ```bash
   # Launch the application
   java --add-opens java.base/java.time=ALL-UNNAMED -cp "bin;lib/gson-2.10.1.jar;lib/jfreechart-1.5.3.jar" Main
   ```

4. **Testing (Optional)**
   ```bash
   # Run TDD test suite
   javac -cp "lib/junit-platform-console-standalone-1.9.2.jar;lib/gson-2.10.1.jar" -d bin test/**/*.java
   java -cp "lib/junit-platform-console-standalone-1.9.2.jar;lib/gson-2.10.1.jar;bin" org.junit.platform.console.ConsoleLauncher --scan-classpath
   ```


---

## 🏆 Project Highlights

### 🎓 **Academic Excellence**
- **Test-Driven Development**: Comprehensive TDD implementation
- **Design Patterns**: MVC architecture with separation of concerns
- **Code Quality**: Well-documented, maintainable codebase
- **Cultural Awareness**: Chinese context integration

### 💡 **Innovation Features**
- **AI-Powered Categorization**: First-of-its-kind Chinese context awareness
- **Cultural Intelligence**: Shopping festival and red packet detection
- **Smart Analytics**: Behavioral pattern recognition
- **User Experience**: Intuitive interface with cultural considerations

### 🔬 **Technical Achievements**
- **Multi-User Architecture**: Scalable user management system
- **Data Integrity**: Robust error handling and validation
- **Performance Optimization**: Efficient data processing and visualization
- **Cross-Platform Compatibility**: Pure Java implementation


---


## 👤 Usage Instructions

1. Run the app, register a new user.
2. Login and add transactions.
3. Check that your data is saved to:
   - `PersonalFinanceTracker/users.json`
   - `PersonalFinanceTracker/transactions_<username>.json`
4. You can import/export CSV and view chart insights.

---

## 👥 Authors

**Group 17 - Queen Mary University of London**

*This project demonstrates advanced software engineering principles including:*
- 🧪 **Test-Driven Development (TDD)**
- 🏗️ **Model-View-Controller (MVC) Architecture**
- 🤖 **Artificial Intelligence Integration**
- 🌍 **Cultural Context Awareness**
- 📊 **Data Visualization and Analytics**



## 📜 License & Academic Use

This project is developed for **academic purposes** as part of coursework at Queen Mary University of London. 

**Features Intellectual Property:**
- AI categorization algorithms
- Chinese context recognition system
- Cultural spending pattern analysis
- Test-driven development methodology
---

<div align="center">

**💡 Ready to transform your financial management experience?**

*Start tracking • Let AI learn • Make informed decisions*

</div>
