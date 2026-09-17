# Jewelry Store Management System

A desktop inventory and sales management application for a jewelry store, built with Java Swing. This was completed as the final project for the Object-Oriented Programming (OOP) course at BINUS University.

## Video Demo

https://youtu.be/ee9vWZVVa6s

## Features

- **Login** — user authentication before accessing the dashboard.
- **Dashboard overview** — at-a-glance stats for earned profit, remaining stock (weight), and total sold jewelries, plus a profit graph.
- **Jewelry list** — browse, add, remove, and search inventory, with checkbox filtering by type (earring, bracelet, ring, necklace, pendant).
- **Purchases & sales** — record jewelry purchases and sales, view purchased/sold data tables.
- **Income statement** — generated income statement table with filtering and search.
- **Calculator** — built-in quick-access calculator.
- **Settings** — application configuration panel.

## Tech Stack

- **Language:** Java
- **UI:** Java Swing (IntelliJ GUI Designer forms) with [FlatLaf](https://www.formdev.com/flatlaf/) look and feel
- **Database:** MySQL (via `mysql-connector-j` / `com.mysql.cj.jdbc.Driver`)

## Project Structure

```
src/
├── Main.java                 # Application entry point
├── LoginMenu.java / .form     # Login screen
├── Dashboard.java / .form     # Main application window
├── Configuration.java         # Database connection configuration
├── Utilities.java              # Shared utility interface
├── Error.java / ErrorInterface.java   # Error dialog handling
├── Dialog.java                 # Reusable dialog windows
├── *_structure.puml            # PlantUML class diagrams
├── Images/                     # Icons and assets
└── flatlaf-3.1.1.jar           # FlatLaf UI library
```

Also included:
- `Class Diagram 1.jpg` — UML class diagram of the system
- `Final Project - OOP - Davin Neilson - 2602119133.pdf` — full project report

## Getting Started

### Prerequisites

- JDK 8+
- MySQL Server running locally
- A MySQL database named `jewelry`

### Setup

1. Create a MySQL database named `jewelry` and set up the required tables/schema.
2. Update the database credentials in [src/Configuration.java](src/Configuration.java) if needed (defaults to `root` with no password on `localhost:3306`).
3. Open the project in an IDE with Swing GUI Designer support (e.g., IntelliJ IDEA).
4. Ensure `flatlaf-3.1.1.jar` and the MySQL Connector/J driver are on the classpath.
5. Run [src/Main.java](src/Main.java).

## Author

Davin Neilson — 2602119133
