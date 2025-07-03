# 📊 Stocks Risk Analysis System

A Java-based desktop application that analyzes the risk level of a stock based on its volatility. The application uses **Swing GUI** for user interaction and stores the analysis results in an **SQLite** database via **JDBC**.

---

## ✅ Features

- GUI input for stock symbol, price, and volatility
- Risk classification as:
  - **Low Risk** (volatility < 0.2)
  - **Medium Risk** (0.2 ≤ volatility < 0.5)
  - **High Risk** (volatility ≥ 0.5)
- Saves analysis to `stocks.db` using JDBC
- Auto-creates the database and table

---

## 📦 Technologies Used

- Java (JDK 8 or above)
- Swing (GUI)
- JDBC
- SQLite

---

## 🛠 How to Run (in Eclipse)

1. **Import Project**
   - File → Import → Existing Projects into Workspace
   - Select the extracted ZIP folder

2. **Add SQLite JDBC JAR**
   - Download from: https://github.com/xerial/sqlite-jdbc/releases
   - Right-click project → Build Path → Configure Build Path → Libraries → Add External JARs → Select `sqlite-jdbc-x.x.x.jar`

3. **Run the App**
   - Run `StocksRiskApp.java` from the `main` package

---

## 📁 Database

- File: `stocks.db`
- Table: `stocks`
- Fields: `symbol` (TEXT), `price` (REAL), `volatility` (REAL), `risk` (TEXT)

---

## 🧪 Sample Input

| Symbol | Price  | Volatility | Risk Output |
|--------|--------|------------|-------------|
| INFY   | 1550.5 | 0.12       | Low Risk    |
| RELI   | 2300.0 | 0.33       | Medium Risk |
| ADANI  | 3750.7 | 0.58       | High Risk   |

---

## 📄 Author

- **Project Name:** Stocks Risk Analysis System
- **Language:** Java
- **Type:** Desktop (Swing + JDBC)
- **Database:** SQLite (embedded, no server required)

---

## 📬 Future Improvements

- Add MySQL/PostgreSQL support
- Export data to CSV/Excel
- View all stock history in GUI
- Add graphs using JFreeChart

