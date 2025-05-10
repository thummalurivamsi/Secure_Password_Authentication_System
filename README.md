# 🔐 Secure Password Authentication System in C

This project is a simple and effective **command-line based password authentication system** written in C. It demonstrates how to handle **secure password input**, **file-based credential storage**, and **basic user validation** using the C standard library.

---

## 📌 Project Overview

Many beginner-level C projects focus on text processing or calculations. This project offers a practical introduction to handling authentication logic in C. It includes features like:

- Username and password matching
- Masking user input with `*` for security
- Reading saved credentials from a file (`password.txt`)
- Re-attempt logic on incorrect entries
- Clear screen functionality for better CLI interaction (Windows)

---

## ⚙ Features

- ✅ Password masking (using `getch()` and `*`)
- ✅ Secure input without echoing actual characters
- ✅ File-based credential storage and retrieval
- ✅ Loops for retrying incorrect username or password
- ✅ Modular and well-commented code

---

## 💻 How It Works

1. The program starts by clearing the console using `system("cls")` (for Windows).
2. It opens `password.txt`, which contains a saved **username and password**.
3. The user is prompted to enter a username:
   - If the username is incorrect, the prompt repeats.
4. If the username is correct, the user is prompted to enter the password:
   - The password input is **masked with asterisks (`*`)**.
   - If the password matches the saved one, a "LOGIN SUCCESSFUL" message is shown.
   - Otherwise, the user is asked to re-enter it.

---

## 🧾 Sample `password.txt` Format

admin
12345

> The first line is the username, and the second line is the password.

---
## 📸 Project Media

![Secure Password Authentication System output](https://github.com/user-attachments/assets/23179d2a-65c8-46c3-948f-d4f52db1f903)


## 🧠 Key Concepts Used

- `fopen()`, `fscanf()` – for file I/O
- `strcmp()` – to compare user input with stored credentials
- `getch()` – to accept characters silently
- `printf("\b \b")` – to handle backspace masking
- `goto` statements – for control flow (can be refactored later)

---

## 📈 Future Improvements
🔐 Add password hashing (e.g., SHA-256) for secure storage

👤 Enable user registration and account creation

🗃 Support multiple user credentials in the file

🔄 Implement password reset functionality

🌐 Make it cross-platform (remove conio.h, use termios.h for Linux)

📊 Add logging of login attempts with timestamps

🧪 Include test cases and modularize code


## 👨‍💻 Developed By

Vamsi T 
Graduate Engineer (ECE) 
vamsithummaluri@gmail.com 

---

## 🛠 License

This project is licensed under the MIT License - feel free to use and modify as needed.

