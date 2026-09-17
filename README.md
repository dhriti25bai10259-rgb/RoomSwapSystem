# Roommate / Room Swapping System

## Project Overview

This is a Java console application for managing hostel students, rooms, and roommate or room swap requests. It demonstrates beginner-friendly object-oriented programming and runs completely from a terminal.

## Problem Being Solved

Manual room swap management can lose requests, allow duplicate processing, and make it difficult to know which rooms are occupied. This project keeps the records organized in memory and lets an administrator process requests safely.

## Objectives

- Manage student and room records.
- Create and track room swap requests.
- Exchange room assignments after admin approval.
- Demonstrate Java and OOP concepts in a simple modular project.

## Features

- Add, view, search, and find students by ID.
- Add rooms, view room status, and check room availability.
- Create, view, accept, and reject swap requests.
- Prevent self-swaps and processing of completed requests.
- Validate numeric input, IDs, names, email, and room numbers.

## Functional Modules

1. **Student Management:** `StudentManager` stores and searches students.
2. **Room Management:** `RoomManager` stores rooms and reports availability.
3. **Room Swap Management:** `SwapManager` creates and processes requests.
4. **Admin Request Management:** `Admin` accepts or rejects pending requests.

## Technologies Used

- Java
- Java Collections Framework (`ArrayList`)
- Command-line interface
- No external libraries, GUI framework, or database

## Project Structure

```text
RoomSwapProject/
├── src/
│   ├── Student.java
│   ├── Room.java
│   ├── SwapRequest.java
│   ├── Admin.java
│   ├── StudentManager.java
│   ├── RoomManager.java
│   ├── SwapManager.java
│   └── RoomSwapSystem.java
├── screenshots/
├── README.md
├── statement.md
├── REPORT.md
└── .gitignore
```

## OOP Concepts Used

- Classes and objects represent students, rooms, requests, managers, and the admin.
- Encapsulation is shown through private fields and public getters/setters.
- Constructors initialize object state.
- Methods contain focused operations.
- Object relationships connect requests to two `Student` objects and the system to managers.
- `ArrayList` stores students, rooms, and requests.
- `if`, `switch`, and loops control decisions and repeated menu work.
- `try-catch` handles invalid numeric input.

## How to Install

Install a Java Development Kit (JDK 8 or later), clone or download this repository, and open a terminal in the project folder.

## How to Compile

```bash
cd RoomSwapProject
javac src/*.java
```

## How to Run

```bash
java -cp src RoomSwapSystem
```

## Testing Instructions

Use the sample data shown when the program starts. Try adding a student, searching by ID or name, creating a request between students `101` and `102`, accepting request `1`, and viewing students again to confirm their rooms were exchanged. Also try an invalid menu choice, a self-swap, and processing request `1` twice.

## Sample Usage

```text
Enter your choice: 6
Enter your Student ID: 101
Enter other student's ID: 102
Swap request created successfully. Request ID: 1

Enter your choice: 8
Enter Request ID: 1
Enter 1 to Accept or 2 to Reject: 1
Room swap successful. Rooms were exchanged.
```

## Future Enhancements

- Save records in a database or file.
- Add login and role-based access.
- Add room capacity and roommate group rules.
- Add a GUI or web client in a separate future version.
- Add automated unit tests and email notifications.

## Author

VITyarthi Build Your Own Project submission
