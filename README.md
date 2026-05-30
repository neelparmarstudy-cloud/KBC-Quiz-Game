# Kaun Banega Crorepati (KBC) Quiz Game

A terminal-based quiz application written in C inspired by the famous television game show *Kaun Banega Crorepati* (Who Wants to Be a Millionaire?). The game incorporates multi-stage progression structures, structural string manipulation configurations to capture user names, and file persistence pipelines to read, validate, and write permanent high scores onto a local file network.

## 🚀 Key Features

### 🎮 Gameplay Architecture
* **Warmup Round (Eligibility Gateway):** Prompts the user with random general knowledge trivia questions. Players must pass a score threshold of at least 2 out of 3 correct answers to gain clearance into the main stadium board.
* **Challenge Round (The Millionaire Run):** Presents a sequence of 10 incremental, continuous-play multiple-choice questions (MCQs). 
* **Dynamic Prize Allocation:** Each accurate terminal response scales the user's prize tier by $100,000, capping out at a grand potential price pool of **$1,000,000 (One Million Dollars)**. A single wrong response safely routes execution down to the score tracking blocks.

### 💾 Core Utility Configurations
* **Permanent High Score Audits:** Integrates disk file pointers (`fopen`, `fclose`) using `score.txt` to safely extract (`fscanf`) and compare local tournament runs. If a new milestone is crossed, the app updates the record stream (`fprintf`) using `w` flags.
* **Live Operational Resets:** Provides a system administrative portal choice to wipe local tracking scores back to zero cleanly.
* **ANSI Terminal Formatting:** Standardizes automated inputs by utilizing `<ctype.h>` utilities to sanitize all key logs into continuous uppercase inputs (`toupper`), preventing minor user casing mistakes from breaking question checkpoints.

---

## 📁 Repository Structure
📁 KBC-Quiz-Game/
│
├── 📄 KBC_game.c             # Core C script containing menu hubs, text databases, and score logic
├── 📄 score.txt              # Local text datastore tracking the highest score and champion player name
├── 📄 .gitignore             # Safeguards local volatile executable runtimes from pushing to Git
├── 📄 LICENSE                # MIT License open-source terms
└── 📄 README.md              # Comprehensive overview documentation
🛠️ Tech Stack
Language: C (C99 standard baseline or higher)
Standard Operating Libraries: <stdio.h>, <conio.h>, <ctype.h>, <stdlib.h>, <string.h>

⚙️ Compilation & Run Guide
To compile and play this interactive game simulation across your workstation terminal:

1. Clone the Repository
Bash
git clone [https://github.com/neelparmarstudy-cloud/KBC-Quiz-Game.git](https://github.com/neelparmarstudy-cloud/KBC-Quiz-Game.git)
cd KBC-Quiz-Game

2. Prepare the High Score Datastore
Before running the executable for the first time, Git requires a placeholder score card to load from. Create a file named score.txt in the same directory and initialize it with a placeholder template entry like this:

Plaintext
Champion 0.00

3. Compile the Source Code
Compile the script using a C compiler (such as gcc or clang):

Bash
gcc KBC_game.c -o KBCGame
Note: This application utilizes platform-specific header libraries like <conio.h> for real-time keystroke listeners (getch()) and internal terminal system overrides (system("cls")), meaning it compiles and executes optimally on Windows terminal systems.

4. Launch the Game Terminal
Execute the compiled binary application block:

DOS
KBC_game.exe
