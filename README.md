# MiniShell Project

## 📌 Project Description
This project is a simple implementation of a **Mini Shell** in C that mimics basic features of a Linux terminal.

It allows users to enter commands, processes them, and executes them just like a real shell.


## ⚙️ Features

### 🧾 Built-in Commands
- `pwd` → Displays the current working directory

- `cd <path>` → Changes the directory
  
- `echo <text>` → Prints text or special variables
  
- `$$` → Prints process ID
 
- `$?` → Prints last command exit status

- `$SHELL` → Prints shell path
 
- `exit` → Exits the shell
 
- `clear` → Clears the terminal screen  

### 🚀 External Commands
- Supports execution of system commands like:
  - `ls`
  - `sleep`
  - `date`
  - and many more using `execvp`

## 🧠 How It Works

1. The shell displays a custom prompt:

2. It takes input from the user.

3. It checks:

- If it's a **built-in command** → executes internally

- If it's an **external command** → executes using system calls  

4. The shell runs in a loop until `exit` is used.

## 🛠️ Technologies Used

- C Programming Language
 
- Linux System Calls
  
- Process Management (`fork`, `exec`, `wait`)  


## 📂 Project Structure

MiniShell/
│
├── main.c

├── scan_input.c

├── main.c

├── header.h

└── README.md


## ▶️ How to Run

# gcc *.c
# ./a.out

# Example output

MiniShell:$ pwd
/home/user/MiniShell

MiniShell:$ echo $$
12345

MiniShell:$ echo Hello World
Hello World

MiniShell:$ cd ..
MiniShell:$ pwd

MiniShell:$ exit
