🎮 Arduino Tic-Tac-Toe Game
OLED Display + 4x4 Keypad | Embedded Systems Project








📌 Project Overview

This project implements a classic Tic-Tac-Toe game using an Arduino Uno, a 4x4 keypad for input, and a 128×64 OLED display for visual output.

Two players can take turns placing their marks (X or O) on the board by pressing keys 1–9 on the keypad. The system dynamically displays:

🎯 Game board

🔄 Player turns

🏆 Winner announcement

The project demonstrates the integration of embedded systems, hardware interfaces, and game logic using Arduino.

📚 Developed as part of the CSE350 Embedded Systems course project

✨ Features

✔ Interactive Tic-Tac-Toe gameplay
✔ OLED graphical game board
✔ Keypad-based player input
✔ Automatic win detection
✔ Two-player gameplay
✔ Turn indicator display

🧠 How the Game Works

The OLED displays a 3×3 Tic-Tac-Toe board.

Players take turns pressing keys 1–9 on the keypad.

Each number corresponds to a board position.

The Arduino updates the board with X or O.

The system checks for:

Row wins

Column wins

Diagonal wins

Once a winner is detected, the OLED displays the winning message.

🧰 Hardware Components
Component	Description
🔹 Arduino Uno	Main microcontroller
🔹 128×64 OLED Display (SSD1306)	Displays the game board
🔹 4x4 Keypad	Player input
🔹 Breadboard	Circuit setup
🔹 Jumper Wires	Hardware connections
📚 Libraries Used

Make sure these Arduino libraries are installed:

SPI.h
Wire.h
Adafruit_GFX.h
Adafruit_SSD1306.h
Keypad.h

You can install them from the Arduino IDE Library Manager.

🔌 Hardware Connection Overview
OLED Display (SSD1306)
OLED Pin	Arduino
VCC	5V
GND	GND
SDA	A4
SCL	A5
Keypad

Connect the 4 row pins and 4 column pins to any available digital pins on the Arduino as defined in the code.

🖥️ Project Structure
Arduino-TicTacToe/
│
├── Arduino_TicTacToe.ino
├── README.md
└── images/
    └── demo.png
▶️ How to Run the Project
1️⃣ Clone the repository
git clone https://github.com/yourusername/Arduino-TicTacToe.git
2️⃣ Open in Arduino IDE

Open the .ino file.

3️⃣ Install Required Libraries

Go to:

Sketch → Include Library → Manage Libraries

Install the libraries listed above.

4️⃣ Upload the Code

Select:

Board → Arduino Uno
Port → Your Arduino Port

Click Upload.

🎮 Gameplay Controls
Key	Action
1-9	Select board position
Players alternate	X → O

Example keypad layout:

1 | 2 | 3
4 | 5 | 6
7 | 8 | 9
📸 Project Demo

(Add your circuit or gameplay images here)

images/demo.png
🚀 Learning Outcomes

Through this project you will learn:

Embedded system design

Hardware interfacing with Arduino

OLED graphics programming

Keypad input handling

Game logic implementation
