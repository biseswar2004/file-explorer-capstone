# 🗂️ File Explorer – Linux Capstone Project (C++)

### 🔧 A Linux-based File Explorer built using **C++17** and **Filesystem Library**

This project replicates the basic functionalities of a Linux shell — allowing users to **navigate**, **create**, **manage**, and **analyze files** directly from a terminal interface.

---

## 📘 Project Overview

This File Explorer is developed as part of the **Linux System Programming Capstone Project**.
The goal is to implement Linux-like commands step-by-step across 5 days — integrating **system calls, directory traversal, file operations, and command utilities**.

The project was implemented, tested, and run inside **WSL2 Ubuntu** using **VS Code**.

---

## 🧠 Key Technologies Used

| Technology        | Purpose                            |
| ----------------- | ---------------------------------- |
| **C++17 STL**     | Core logic and filesystem handling |
| **<filesystem>**  | File and directory management      |
| **WSL2 (Ubuntu)** | Linux environment for execution    |
| **Makefile**      | Build automation                   |
| **Git & GitHub**  | Version control and documentation  |

---

## 🗓️ Day-wise Development Progress

### 🟩 **Day 1 – Basic Setup & File Listing**

**Objective:** Initialize the project and add basic shell commands.
**Commands Implemented:**

* `pwd` → Print current working directory
* `ls` → List files and directories
* `exit` → Exit the explorer

**Highlights:**

* Basic terminal UI created
* Setup `Makefile` for build automation
* Verified environment with WSL2 and Git integration

📂 *Commit:* `Day1: Basic setup with ls and pwd commands`

---

### 🟨 **Day 2 – Directory Navigation & File Creation**

**Objective:** Enable navigation and basic file/directory creation.
**Commands Added:**

* `cd <dir>` → Change directory
* `mkdir <dir>` → Create directory
* `touch <file>` → Create new file

**Highlights:**

* Introduced `std::filesystem::current_path()`
* Implemented exception handling for invalid paths
* Practiced user interaction and path validation

📂 *Commit:* `Day2: Added cd, mkdir, and touch commands for navigation`

---

### 🟦 **Day 3 – File Manipulation & Info Retrieval**

**Objective:** Manage and analyze files.
**Commands Added:**

* `cp <src> <dest>` → Copy file
* `mv <src> <dest>` → Move or rename file
* `rm <file>` → Delete file/folder
* `info <file>` → Display file type, size, and modified time

**Highlights:**

* Integrated `std::filesystem::copy`, `rename`, `remove`
* Introduced `chrono` for timestamp formatting
* Handled permission and missing file errors gracefully

📂 *Commit:* `Day3: Added cp, mv, rm, and info commands`

---

### 🟪 **Day 4 – Search, Tree View & Help System**

**Objective:** Add exploration and documentation features.
**Commands Added:**

* `find <name>` → Search for files/directories recursively
* `tree` → Display directory structure recursively
* `help` → List all available commands

**Highlights:**

* Used recursive iterators for deep traversal
* Created a beautiful `tree` visualization
* Added an in-program help guide for users

📂 *Commit:* `Day4: Added find, tree, and help commands for search and navigation`

---

### 🟥 **Day 5 – History, Clear & Exit Confirmation**

**Objective:** Polish UI and improve user experience.
**Commands Added:**

* `history` → Show all executed commands
* `clear` → Clear the terminal screen
* `exit` → Added confirmation (`Are you sure? y/n`)

**Highlights:**

* Implemented vector-based command history
* Integrated `system("clear")` for screen refresh
* Completed final build and cleanup with `.gitignore`

📂 *Commit:* `Day5: Added history, clear, and exit confirmation - Final Build`

---

## 🧩 Project Structure

```
file-explorer-capstone/
├── Day1/                     # Day 1 version code
├── Day2/                     # Day 2 version code
├── Day3/                     # Day 3 version code
├── Day4/                     # Day 4 version code
├── Day5/                     # Final version
├── demo_session/             # Screenshots or demo recordings
├── src/
│   └── file_explorer.cpp     # Active development file
├── Makefile                  # Build automation script
├── .gitignore                # Ignored files configuration
└── README.md                 # Project documentation
```

---

## 💻 How to Build & Run

### 🧰 Prerequisites

* Ubuntu (via WSL2)
* g++ compiler (C++17)
* make utility
* Git installed

### 🛠️ Build

```bash
make
```

### ▶️ Run

```bash
./file_explorer
```

### 🧹 Clean

```bash
make clean
```

---

## 🧪 Example Demo Commands

```bash
pwd
ls
mkdir demo
cd demo
touch hello.txt
cp hello.txt copy.txt
info copy.txt
tree
find hello
history
exit
```

---

## 📸 Demo Session

All screenshots and run logs are stored in the `demo_session/` folder.
Example files:

```
demo_session/
 ├── day1_output.png
 ├── day2_demo.png
 ├── day3_operations.png
 ├── day4_search_tree.png
 └── day5_final.png
```

---

## ⚙️ .gitignore Highlights

```gitignore
file_explorer
*.o
*.out
*.log
/build/
/temp/
/cache/
```

This ensures compiled files don’t clutter your repository.

---

## 🌟 Final Output Preview

```
Simple File Explorer - Final Build
Type 'help' for list of commands.

/home/biseswar/projects/file-explorer-capstone $
Commands: pwd, ls, cd, mkdir, touch, cp, mv, rm, info, find, tree, history, clear, help, exit
```

---

## 👨‍💻 Author

**Biseswar Mohapatra**
🎓 Linux System Programming | C++ Developer | Automation Enthusiast
📧 [biseswarmohapatra@gmail.com](mailto:biseswarmohapatra214@gmail.com)
🌐 [GitHub Profile](https://github.com/biseswar2004)

---

## 🏁 Conclusion

This project successfully demonstrates:

* Mastery of Linux filesystem operations in C++
* Use of modern C++17 features and robust error handling
* Real-world application of system programming concepts
* Professional GitHub documentation and structure

🎉 **Project Completed: 100% Functional (Day 1 → Day 5)**
